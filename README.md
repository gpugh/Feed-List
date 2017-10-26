# Feed-List
Feature: Display RSS feed(s)
  Ability to show Photo or News feed
  Module must be placed on desired page
  User must be in edit mode to configure
  Feed List must be configured to display
  
  Scenario: User configures module
    Given User is logged in
    And They are in edit mode
    When the user mouses over pencil icon in the top right of module
    And Selects the FeedList Admin
    When the settings load and user enters desired RSS URL
    And selects their branch
    And chooses branch Template
    And selects description
    And selects desired choice for Open in a new window
    And clicks update
    And clicks return
    Then RSS feed will display on site
    And viewers of site will be able to select RSS feeds from module

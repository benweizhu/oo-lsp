# oo-lsp

```gherkin
Feature: 
    Scenario: Shoot
    
    Given I have a 98k 
    And 5 "762 bullet" loaded
    When I fire
    Then 1 "762 bullet" shoot out
    
    Given I have a 98k 
    And no "762 bullet" loaded
    When I fire
    Then no "762 bullet" shoot out    

    Scenario: Reload
    
    Given I have a 98k 
    And 0 "762 bullet" loaded
    And 30 "762 bullet" available
    When I reload
    Then 5 "762 bullet" reloaded
    
    Given I have a 98k 
    And 0 "762 bullet" loaded
    And 4 "762 bullet" available
    When I reload
    Then 4 "762 bullet" reloaded    
    
    Given I have a 98k 
    And 5 "762 bullet" loaded
    And 30 "762 bullet" available
    When I reload
    Then No "762 bullet" reloaded
    
    Given I have a 98k 
    And 0 "762 bullet" loaded
    And 0 "762 bullet" available
    When I reload
    Then No "762 bullet" reloaded    
```
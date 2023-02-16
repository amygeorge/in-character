# in-character
##  Motivation: 
#### Sometimes you want to read fan fiction about your favourite character(s) but you don't want to write it yourself. You want a specific set-up and you want the story to be canon accurate. 
## Goal: 
#### Generate a short story (500 words) based on user input (character name and tags from AO3)

## Project Requirements:
### Data:
- Narrow down data by fandom, character
- Scrape AO3
  - Script characters by in-built tag system
    - Script to eliminate multi-character works
      - Script across multiple chapters of a given work via the full-story view
      - or limit to stories within a given word range (say 500-1500)
  - Script tags system for set up
- Store data in cloud
  - Choose cloud platform that 
    - Is affordable or free
    - Can run NLP models 
    - Azure?
    
### Generative Model:
- Research generative models
  - Models must be able to:
    - Gather information from across large spans of text about a given topic (character)
      - Physical description, personality, common background information, world building (?)
        - Text window around character name to extract pertinent information
        - Bag of words from that data to find most common details
        - Somehow simplify the story input to focus only on character details, not everything
    - Generate natural literature appropriate text
      - Learn style from stories?
    - Use tags to ensure desired events occur in generated story
      - Use tags information as part of input with story text and create vectors of information
        - Masking?
      - Learn across vectors with same tags to inform text generation, aka story set-up
- Ultimate goal is to generate situations for (somewhat) novel characters
  - Known tags trained on other characters used for new character 

### Literature Review
- [Spinning Coherent Interactive Fiction through Foundation Model Prompts](https://computationalcreativity.net/iccc22/wp-content/uploads/2022/06/ICCC-2022_2L_Calderwood-et-al..pdf)


### Keywords
#### Natural Language Processing (NLP), Automated Story Generation (ASG), 

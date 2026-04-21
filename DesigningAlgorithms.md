# Structure Charts

<img width="386" height="585" alt="Screenshot 2026-04-21 at 2 26 59 pm" src="https://github.com/user-attachments/assets/595117ec-028a-499a-bf31-c9606b55daff" />

# Pseudo Code
START

DISPLAY homepage

WHILE user is on website DO

    DISPLAY search bar and term list
    
    GET user_input
    
    IF user_input is not empty THEN
        
        IF term exists in database THEN
            RETRIEVE term_definition
            RETRIEVE analogy
            RETRIEVE code_example
            RETRIEVE visuals
            
            DISPLAY all information
            
            DISPLAY options:
                1. Bookmark
                2. Take Quiz
                3. New Search
            
            GET user_choice
            
            IF user_choice = Bookmark THEN
                SAVE term to user bookmarks
                DISPLAY "Saved!"
            
            ELSE IF user_choice = Quiz THEN
                DISPLAY quiz questions
                GET answers
                CHECK answers
                DISPLAY score
            
            ELSE IF user_choice = New Search THEN
                CONTINUE loop
            
        ELSE
            DISPLAY "Term not found"
            DISPLAY similar_terms
        ENDIF
    
    ENDIF

ENDWHILE

END

CSS Grid

https://www.youtube.com/watch?v=EFafSYg-PkI



    grid-template-columns
    grid-template-rows
      px = pixels
      % = percentaje
      fr = fractions (1 = the available space)
      
     
     
    grid-column-start
    grid-column-end
        1 = top left
        2 = in between the 1st and the 2nd columns
        3 = in between the 2nd and the 3rd columns
        ...

        On this example and since there are just 2 columns, 
        "3" would be the top right
        ALSO, you can go for -> 
        grid-column-start: 1;
        grid-column-end: 3;
        OR ->
        grid-column: 1/3;
    AND THE SAME WAY FOR "grid-row"
        
        
        
    Another way would be using "grid-template-areas" 
    .box1 {grid-area: primero;}
    .box2 {grid-area: segundo;}
    .box3 {grid-area: tercero;}
    
    grid-template-areas: 
    "primero tercero"
    ". segundo";
    
    
    
    This is how we make a responsible grid:
    "grid-template-columns: repeat(3, 600px);" means three 600pixels columns.
    "grid-template-columns: repeat(auto-fit, 600px);" means the max amount of 600 pixels columns.
    "grid-template-columns: repeat(auto-fit, minmax(300px, 1fr);" means the max amount of columns, considering that columns cannot be less than 300 pixels.
    
    
    
    As a side note, you can add a gap in between rows and columns.
    grid-column-gap: 15px;
    grid-row-gap: 15px;

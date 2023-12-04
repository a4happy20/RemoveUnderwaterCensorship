# RemoveUnderwaterCensorship
   
### Requirements:
  1. 3dmigoto GIMI
    
    
#### Description:
  INI file for globally tracking when the character is in/underwater. Also removes underwater censorship at all resolutions.

#### Update:

       
     
##### How to Use:
  1. Place in the BufferValues folder located at 3dmigoto "Mods" folder.
  2. Recomended to use "autoUnderwaterOutfit.py" (If not see step 3).
  3. Insert into the ini you want to detect water
     ```
     [Constants]
     global $submerged_start
     global $active (only if not present already)
     
     [Present]
     if $active == 1
        $submerged_start = $\global\submerged\submerged_start
     endif

     [TextureOverride"your character"Position]
     $active == 1
     ```
      
      
##### Additional Information:
  1. Required for "autoUnderwaterOutfit.py"

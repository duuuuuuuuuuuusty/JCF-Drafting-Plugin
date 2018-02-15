# JCF Drafting Plugin
For JC Ink services

Version 1.02

## Installation
Add the file to your forum wrappers - I recommend using a webpage and the include key to keep your wrappers tidy. The file uploading row in the add post or new topic forms is automatically removed, as it conflicts with the script's functionality.

## Usage
The script appends a new row to the posting form (quick reply functionality not yet included). Clicking the _Save_ button will format and save the post body (and title and description, if posting a new topic) and prepend the data to the UCP notepad, as well as update the draft selection menu. The script will also run an autosave function every 5 seconds (configurable at the bottom of the script), which will save a draft named after the time of page creation if the savename input field is not filled in. The autosave feature will suspend for as long as the savename input has focus, to prevent some accidental overwrites.

The selection menu will populate on load with all saved drafts of a matching type: only posts will show up when posting a new reply, and only topics will show up when posting a new topic. Selecting an option will load its contents into the preview box, which can then be moved into the post body by clicking the _Send to Post_ button.

## Common Troubleshooting
1. Preview box appears empty
  The preview box may appear empty on the first execution of the script with a blank notepad.
  
2. Certain drafts are not appearing
  Check the UCP notepad and ensure that each draft (indicated by wrapping {post} or {topic} tags) is separated via at least one newline. If two separate tags occupy the same line, eg: {/topic}{post}, the script will not correctly parse them as separate.

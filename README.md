# JCF Drafting Plugin
For JC Ink services

Version 0.1 (BETA)

## Installation
Add the file to your forum wrappers - I recommend using a webpage and the include key to keep your wrappers tidy. For the time being, in order to get full functionality for saving topics, you must disable the file attachment system in the boards you want to use the drafting on. You can do this via the permissions masks.

## Usage
The script appends a new row to the posting form (quick reply functionality not yet included). Clicking the _Save_ button will format and save the post body (and title and description, if posting a new topic) and prepend the data to the UCP notepad, as well as update the draft selection menu.

The selection menu will populate on load with all saved drafts of a matching type: only posts will show up when posting a new reply, and only topics will show up when posting a new topic. Selecting an option will load its contents into the preview box, which can then be moved into the post body by clicking the _Send to Post_ button.

## Common Troubleshooting
1. Preview box appears empty
  The preview box may appear empty on the first execution of the script with a blank notepad.
  
2. Certain drafts are not appearing
  Check the UCP notepad and ensure that each draft (indicated by wrapping {post} or {topic} tags) is separated via at least one newline. If two separate tags occupy the same line, eg: {/topic}{post}, the script will not correctly parse them as separate.

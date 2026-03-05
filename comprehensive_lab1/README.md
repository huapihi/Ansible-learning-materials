# Notes/Recommendations

## Project folder 
There are several ways to structure a project when it comes to ansible.  It really depends on your use case and whether it's a standalone project or a collection.  
Your project folder name should be considered the "root" of the project.  In your case you created the Ansible-Learning-Materials(ALM) repo and then created your Ansible project underneath.  Just keep that in mind.   
For now, it will make things easier for us as you learn and we'll create separate "projects" within the ALM repo.  

Your structure is starting out like a hybrid between a role and a typical Ansible folder structure. It's not "bad" per se, but there is room for improvement so it more closely aligns with what you may see in a typical environment. 

See this document reference for more of what I'm talking about:

https://docs.ansible.com/projects/ansible/latest/tips_tricks/sample_setup.html


## Inventory
You have two hosts in your inventory, but they're not grouped.  This isn't necessarily bad, but you should group your hosts when possible.  There are also two ansible specfic groups which are called "all" and "ungrouped".  All = all hosts and ungrouped are hosts that are not part of any group. So based on your inventory, your hosts would be in the ungrouped group.  I dont' want to go into too deep of waters, but want to at least let you know about them.
Lastly, comfortable with yaml based inventories as quickly as possible.  INI formatted  inventories are limited.  You can't do dictionaries or lists or secrets within them.  In a yaml format, there are endless possibilities.

## lab_main.yml
See the file itself.  Lots of notes there

## Tasks playbooks
Not sure what you're trying to do since they look like you would be including them as a part of a larger playbook.  



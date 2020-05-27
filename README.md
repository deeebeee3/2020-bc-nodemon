Add to top of index.js to allow it to be treated like an executable:
#!/usr/bin/env node 

Give permission to run file as though it were an executable:
chmod +x index.js

Create package.json:
npm init -y


We want to be able to type the command "watchit" at the terminal
and run index.js as though it were some kind of executable (add to package.json):

"bin": {
    "watchit": "index.js"
}

Make our current project globally available in every directory and everywhere else:
npm link

See docs:
watchit -h
# End assignment
## Contineous Deployment with Github Actions

For a final assignment I didn't have as much trouble as I thought I would.
Of course I had to revisit some of the previous exercises, but didn't ran into problems that I couldn't resolve easily.

I used Digital Ocean to create a VPS and run my project through a server.<br>
In VS Code I created the files and then copied the directory into the VPS.<br>
In cooperation with Google, it was fairly easy to create read-only access. Also working with *secrets* wasn't too hard to figure out.<br>
On Github I created 3 repository secrets:
- SSH_HOST
- SSH_KEY
- SSH_USERNAME

And then added these to the `run-test.yml` file in the section `deploy`.
<br>
I did struggle a bit with this error:
 ```
 error: Connection In Use (‘127.0.0.1’, 8000)
 ```
Apparently there still was another flask application listening to the same port, but I found out which on and killed it.
After this fix, it was possible to deploy automatically after tests pass with Github Actions.


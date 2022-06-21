# End assignment
## Contineous Deployment with Github Actions

For a final assignment I didn't have as much trouble as I thought I would.
Of course I had to revisit some of the previous exercises, but ran into little problems that I couldn't resolve easily.
In cooperation with Google, it was fairly easy to create read-only access. Also working with *secrets* wasn't too hard to figure out. 

I've created 3 repository secrets:
- SSH_HOST
- SSH_KEY
- SSH_USERNAME

And then added these to the `run-test.yml` file.
I did struggle a bit with an error:
 ```
 error: Connection In Use (‘127.0.0.1’, 8000)
 ```
Apparently there still was another flask application listening to the same port.



tbc....

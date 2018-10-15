#Github setup for collaborators
##Overview:
Collaborators are added to each repo and once the invitation is accepted, collaboration can begin updating the contents of the repo.
Some important points:
1. Collaborator must always use their own userid/pwd to login.  This means using the https git repo url (which requires userid/pwd). Collaborator ssh keys should not be uploaded to the repo.  The ssh key method does not require userid/pwd.
2. For repos that need to be controlled more, use the Github option to protect branches:

* master branch should be protected (push/merge requires review)
* Create branch for collaborator (name it VV)
* Collaborator should checkout only that specific branch using:
  1. git clone -b VV --single-branch https://github.com/arjunvasan/tts.git --depth 1
  This helps in working only in that branch



# CI/CD 
 
1. Fork this Repository.
2. Start a new ubuntu vm.
3. Install docker and zsh:
```bash
curl https://raw.githubusercontent.com/ics-unisg/cicd/main/get-scs-base.sh | sh
```
4. Define SSH_HOST, SSH_PRIVATE_KEY and SSH_USER.

SSH_USER is the username

SSH_HOST is the ip address of the vm

SSH_PRIVATE_KEY is the private key for the user that has admin rights on that vm

Make sure your sshd_conf accepts the key: https://www.deployhq.com/support/common-server-errors/ssh-rsa-not-in-pubkeyacceptedalgorithms 

![image](https://user-images.githubusercontent.com/2293142/121609248-c324d780-ca53-11eb-9929-1a14d34ccba9.png)

5. Push new code to the main branch
6. Open in your browser `https://app.<server-ip>.nip.io` changing all dots in `<server-ip>` into - i.e. `app.192-168-1-1.nip.io`

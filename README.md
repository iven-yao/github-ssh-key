# Generate public key
[Official Tutorial](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
- in command line use following to create a public key in ~/.ssh/id_ed25519.pub
  
  `ssh-keygen -t ed25519 -C "your_email@example.com"`

- if first time, should setup ssh agent and key chain, check tutorials ^

# Adding an SSH key on github with public key
[Official Tutorial](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account?tool=webui)
- copy the public key with

  `pbcopy < ~/.ssh/id_ed25519.pub`

- go to github > Settings > Access - SSH and GPG keys
- New SSH keys, paste the public key in Key section

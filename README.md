# Global post-checkout hook to automatically set local user configuration of a repo, when cloning from a specific host

1. Enable Git hooks globally:
   
   ```bash
   git config --global init.templatedir '~/.git-templates'
   ```

2. Create the post-checkout hook
   
   ```bash
   mkdir -p ~/.git-templates/hooks
   cp post-checkout ~/.git-templates/hooks/post-checkout
   chmod +x ~/.git-templates/hooks/post-checkout
   ```

3. Edit the hook-file to insert your credentials and specific host
   
   ```bash
   vim ~/.git-templates/hooks/post-checkout
   ```



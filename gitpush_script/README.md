```bash
vim /.bashrc

gitpush() {
    read -p "commit message: " comment
    git add .
    git commit -m "$comment"
    git push
}


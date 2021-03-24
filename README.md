# terraform-action

Literally just the 0.14.9 binary in a container, nothing more, nothing less!

Example usage, e.g. a terraform plan:
```
    - name: Terraform Plan
      uses: gvillalta99/terraform-action@v0.14.9
      with:
        args: "plan -var-file=vars/dev.tfvars"
      env:
        AWS_ACCESS_KEY_ID: ${{ secrets.AWS_ACCESS_KEY_ID }}
        AWS_SECRET_ACCESS_KEY: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
```

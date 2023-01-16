# docker-run-tools
This is a collection of tools runnable using docker. This is a demo that execute the plan command 


## Terraform

Run the following command in the terraform home project

```bash
docker run --rm -it -w /$(basename $(pwd)) -v $(pwd):/$(basename $(pwd)) -v $HOME/.aws/:/home/root/.aws/ -v ~/.aws:/root/.aws  hashicorp/terraform:1.3.6 plan```

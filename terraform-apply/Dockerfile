FROM hashicorp/terraform:0.11.13

LABEL "com.github.actions.name"="terraform apply"
LABEL "com.github.actions.description"="Run Terraform Apply"
LABEL "com.github.actions.icon"="upload"
LABEL "com.github.actions.color"="purple"

LABEL "repository"="https://github.com/samelogic/github-actions"
LABEL "homepage"="http://github.com/samelogic/github-actions"
LABEL "maintainer"="Samelogic <shawn@samelogic.com>"

RUN apk --no-cache add jq

COPY entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]

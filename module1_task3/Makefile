help: ## Show command help
	@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\\$$//' | sed -e 's/##//'

build: ## Generate the website from the markdown and configuration files in the directory dist/
	hugo

clean: ## Cleanup the content of the directory dist/
	rm -rf dist/

post: ## Create a new blog post whose filename and title come from the environment variables POST_TITLE and POST_NAME
	hugo new posts/$(POST_NAME).md && echo "---\ntitle: \"$(POST_TITLE)\"\ndate: 2023-05-04T15:14:01+02:00\ndraft: true\n---" > content/posts/$(POST_NAME).md

build:
	hugo
clean:
	rm -rf dist/
post:
	hugo new posts/$(POST_NAME).md && echo "---\ntitle: \"$(POST_TITLE)\"\ndate: 2023-05-04T15:14:01+02:00\ndraft: true\n---" > content/posts/$(POST_NAME).md

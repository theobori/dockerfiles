TAG_MAJOR=true

# define default action, implemented in Makefile.mk
build:

pre-push:
	docker tag andrewmackrodt/nodejs:14 andrewmackrodt/nodejs:maintenance
	docker tag andrewmackrodt/nodejs:16 andrewmackrodt/nodejs:lts
	docker tag andrewmackrodt/nodejs:18 andrewmackrodt/nodejs:current

post-push:
	docker push andrewmackrodt/nodejs:maintenance
	docker push andrewmackrodt/nodejs:lts
	docker push andrewmackrodt/nodejs:current

include ../Makefile.mk

# A Simple Cypress Template Demo with Docker Image Ready to be built



This Simple Repository have the cypress installed and and `Dockerfile`  with the cypress image `cypress/included:3.4.0` .

### The `Dockerfile` used:

```dockerfile
FROM cypress/included:3.4.0
WORKDIR /home/cypress-app
COPY app /home/cypress-app
RUN npm install
CMD npm run test
```

### Installation 

You will just need to clone this repository and run the build the image and use it.

```
git clone https://github.com/MoatazFarid/simple-cypress-with-docker-template.git
```

**Build  the Image**

```
docker image build --tag cypress-docker-template/demo .
```

That's It :) .

**Todo:**

- [ ] Add locators cypress plugins 
- [ ] Add reporting cypress plugins 
- [ ] Add Proper CI GitHub Actions script 


# API Design workshop


## Step1. Let's describe what actions our API affords

- Retreive my videos
- Create a new video
- Update a specific video
- Get a specific video
- Share a video
- Delete a video

## Step2. Let's create our state machine diagram


![Video Model state diagram](https://raw.githubusercontent.com/Amzani/api-lifecycle-tutorial/master/img/State_Diagram.png)

This state machine diagram will help you to identify the main ressources and their relations.

## Step3. Formalize the design in the [Open API Specification](http://swagger.io/specification/)


[Swagger](./swagger.yml)
[Documentation](https://playvideoapi.docs.apiary.io)


## Develop the API

### Dev workflow

1. Clone this [repo](https://tools.adidas-group.com/bitbucket/users/amzansam/repos/demo-video-api/) (internal)
2. Test with dredd
3. Add This endpoint to your OAS file
```
  /foo:
    x-summary: Foo

    get:
      summary: The FOO action
      description: Retrieve the Foo

      responses:
        200:
          description: Foo
          type: string
```
4. Run dredd again




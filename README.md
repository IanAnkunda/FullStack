# FullStackLabs
# Introduction

You will create a screen recording video of yourself completing the challenge, then send me a link to the file via Google Drive. A few things to consider:

- We ask that you complete this challenge within the timeframe agreed on in our conversation.
- **You MUST NOT edit your video, stop it and continue later, copy contents from hidden screens, or anything similar that can be considered cheating. The recording must be without stopping and no editing.**
- You can use screen recording software like Loom, QuickTime, or something similar, to create the video.
- The recording should be of the entire coding challenge, from the beginning to end, which is about 1 hour and 15 minutes.
- Please upload the video file to Google Drive and share an open link with us (we support .mp4, files smaller/with less than 4gb).
- As you complete the challenge, please explain what you are doing. Walk us through your thinking, explain your decisions, etc. Show us your UI work, if applicable.
- Here is a short clip from a recent coding challenge, as an example of what your recording should look like: [Example video](http://www.loom.com/share/85434243d487456b8ef4ae45c3fbc788). It is from a React challenge, but it is the same for any challenge.

## **Challenge**

This API manages bags and cuboids. A cuboid is a three-dimensional rectangular box. Each face of a cuboid is a rectangle and adjacent faces meet at right angles. A cube is a cuboid with equal dimensions. A cuboid has a volume that is straightforward to calculate.

A bag is a malleable container with adjustable dimensions, but a fixed volume. The bag can expand to hold any shape or combination of shapes, but the volume of the bag is limited and cannot expand. In our model a bag has many cuboids.

This app has an almost complete test suite.

The tests to update and delete a cuboid are incomplete, your task is to improve them.

The other tests are valid and you must not modify them. In other words, you need to add the missing functionalities so that these tests pass.

You should also take note of PMD. The PMD is currently passing and must pass on completion of the challenge, without any modifications to the config.

**Note**:

1. The only tests to be modified are tests to update and delete a cuboid. All other tests must remain unchanged.
2. The controller tests are using real service and DB (H2 database). Some of them are broken due to inconsistency with DB.
3. You should fix these problems related to database, according to the controllers tests, using flyway.

## Steps

To participate in this challenge take the following steps:

1. Clone this repository.
2. Checkout a feature branch where you will make your changes.
3. Setup the app and get it running. Verify that the linter passes and the test suite fails.
4. Implement tests to update and delete a cuboid.
5. Add missing functionalities so the other tests pass. Do NOT modify these tests.
6. Commit as appropriate as you complete the challenge. (More than one commit is expected)

## **Technology**

This app uses the following key technologies:

- [Java 11](https://www.oracle.com/java/technologies/downloads/)
- [Maven 3.8.3](https://maven.apache.org/download.cgi)

## **Setup**

Create `JAVA_HOME` and add the `bin` directory of maven to the PATH in the environment variables Use the following command to install the dependencies:

```bash
mvn -Dmaven.test.skip=true clean instal
```

## **Usage**

Run the app (Or you can run in your IDE):

```bash
mvn spring-boot:run
```

Run the PMD:

```bash
mvn pmd:pmd
```

Run the tests:

```bash
mvn test
```

# README

A ruby on rails API based on the tutorial from https://medium.com/the-era-of-apis/how-to-build-a-restful-api-in-ruby-8265f1c47b72

run:
1. run rails server: "rails s"
2. type the following command in console:
    curl localhost:3000/say \
      -H 'Content-Type: application/json' \
      -d '{"message": "Hello from RapidAPI", "cow": "stegosaurus", "balloon_type": "think"}' \
    | ruby -r json -e "print JSON.parse(STDIN.read)['message']"

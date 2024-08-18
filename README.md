# Twitter DApp

This is a decentralized Twitter-like application built on the Ethereum blockchain. The smart contract allows users to create, like, and unlike tweets, with user profiles managed through an external profile contract.

## Features

- **Create Tweets**: Users can post tweets with a maximum length of 280 characters (configurable by the owner).
- **Like/Unlike Tweets**: Users can like or unlike tweets, and each tweet tracks its like count.
- **User Profiles**: Only registered users (with profiles) can interact with the contract.
- **Profile Integration**: The contract integrates with an external profile contract to manage user details like display name and bio.
- **Owner Controls**: The contract owner can modify the maximum tweet length.

## Getting Started

### Prerequisites

- Solidity `^0.8.0`
- OpenZeppelin contracts (Ownable)

### Deployment

Deploy the `Twitter` contract by passing the address of the profile contract during deployment.

### Usage

1. **Register a Profile**: Users must have a profile set up in the external profile contract to create or interact with tweets.
2. **Create a Tweet**: Use the `createTweet` function to post a tweet.
3. **Like/Unlike a Tweet**: Use the `likeTweet` and `unlikeTweet` functions to like or unlike tweets.
4. **View Tweets**: Retrieve individual tweets or all tweets by a user with `getTweet` and `getAllTweets`.

## License

This project is licensed under the MIT License.

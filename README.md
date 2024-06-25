# Privyfit

PrivyFit: Privacy-Focused Social Fitness App

Goal Setting:
* Users set their target weight and deadline.
* This information is encrypted and stored.
1. Initial Weight Recording:
   * Users record their starting weight.
   * This information is also encrypted and stored.
2. Daily Weight Recording:
   * Users regularly (daily or weekly) record their weight.
   * All records are encrypted and stored.
3. Progress Check Towards Goal:
   * The system uses encrypted data to determine if the user is on track to their goal.
   * This determination considers current weight, initial weight, target weight, elapsed time, and set deadline.
4. Zero-Knowledge Proof Generation:
   * The system proves the fact that "the user is on track towards their goal" or "the user is off track".
   * When the target weight is reached, the system generates a proof of achievement.
   * These proofs do not include specific weight numbers.
5. Progress Sharing on Social Media:
   * Users can share their progress proofs on social media platforms.
   * The shared information states whether they are "on track", "off track", or have "reached their goal".
   * Users can regularly update their progress without revealing actual weights.
   * When the target is reached, users can proudly announce their achievement while maintaining privacy.
6. Social Interaction:
   * Other users can view and interact with shared progress updates.
   * The community can offer support and encouragement based on these privacy-preserving updates.
   * 
Advantages of this approach:
1. Privacy Protection: Progress can be shared without revealing specific weights.
2. Motivation Maintenance: Being able to prove progress towards the goal can boost motivation.
3. Social Support: Users can engage with a supportive community while maintaining privacy.
4. Achievement Celebration: Users can proudly share their success when reaching their goal, without disclosing actual numbers.
5. Simplicity: The information shared is easy to understand and relate to for other users.
6. Trustworthiness: Zero-knowledge proofs ensure that achievements are verifiable without compromising privacy.
This project caters to individuals who want to share their diet progress and achievements on social media but are hesitant to disclose their actual weight. By utilizing zero-knowledge proofs, users can effectively communicate their success, maintain accountability, and celebrate achievements within a supportive community, all while keeping their sensitive information private.


## Update ( 2024/06/25）

User Interface:

The user interacts with the Frontend, which includes features for authentication, weight recording, goal setting, progress sharing, and community interaction.

![userinterface](https://github.com/harucoinlove/Privyfit/blob/main/assets/frontend.png)

Backend:

The Backend API handles user management, data management, zero-knowledge proof generation, and progress verification.
It communicates with both the database for data storage and the Mina Protocol node for blockchain interactions.

![backend](https://github.com/harucoinlove/Privyfit/blob/main/assets/backend.png)

Mina Protocol Integration:

The Mina Protocol node hosts the smart contract and performs zero-knowledge proof verification.

![minaprotocol](https://github.com/harucoinlove/Privyfit/blob/main/assets/mina.png)
Data Flow:

User data and interactions flow from the Frontend to the Backend API.
The Backend API processes this data, interacts with the database, and communicates with the Mina Protocol node as needed.

![dataflowimage](https://github.com/harucoinlove/Privyfit/blob/main/assets/dataflow.png)


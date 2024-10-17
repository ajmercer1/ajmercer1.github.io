flowchart TD
    A([Start]) --> B[("Get a Random Number (1-100)")]
    B --> C[("Ask User for a Guess")]
    C --> D[("Is the Guess Valid?")]
    D -->|Yes| E[("Check if Guess is Right")]
    D -->|No| C
    E -->|Too High| F[("Say: Too High! Try Again.")]
    E -->|Too Low| G[("Say: Too Low! Try Again.")]
    E -->|Correct| H[(" You got it!")]
    F --> C
    G --> C
    H --> I([End])

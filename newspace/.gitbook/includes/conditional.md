---
title: conditional
---

<a href="../../" class="button secondary" data-icon="android">Android</a> <a href="/broken/pages/0lPKgkWxFagLn6BSuxXb" class="button primary" data-icon="apple">Apple</a>&#x20;



Swift Code:

```swift
import SwiftUI

struct ContentView: View {
    var body: some View {
        VStack {
            // Basic button
            Button("Tap Me") {
                print("Button tapped!")
            }
            .buttonStyle(.borderedProminent)
            
            // Custom styled button
            Button(action: {
                // Handle button tap
                handleButtonTap()
            }) {
                Text("Custom Button")
                    .font(.headline)
                    .foregroundColor(.white)
                    .padding()
                    .background(Color.blue)
                    .cornerRadius(10)
            }
        }
    }
    
    func handleButtonTap() {
        print("Custom button was tapped!")
    }
}
```

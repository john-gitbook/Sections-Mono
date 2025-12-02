---
title: import SwiftUIstruct Conten...
---

{% if  %}
```swift


 SwiftUI

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
{% endif %}

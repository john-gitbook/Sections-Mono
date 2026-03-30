# Conditional Content

Welcome, select your option below:

{% if visitor.claims.unsigned.example_android == "android" %}
<a href="https://support-examples.gitbook.io/conditions/?visitor.example_android=android" class="button primary" data-icon="android">Android</a> <a href="https://support-examples.gitbook.io/conditions/?visitor.example_android=apple" class="button secondary" data-icon="apple">Apple</a> <a href="https://support-examples.gitbook.io/conditions/?visitor.example_android=ubuntu" class="button secondary" data-icon="ubuntu">Ubuntu</a>



Kotlin Code:

```kotlin

import androidx.compose.foundation.layout.*
import androidx.compose.material3.*
import androidx.compose.runtime.Composable
import androidx.compose.ui.Alignment
import androidx.compose.ui.Modifier
import androidx.compose.ui.unit.dp

@Composable
fun ButtonExample() {
    Column(
        modifier = Modifier.fillMaxSize(),
        horizontalAlignment = Alignment.CenterHorizontally,
        verticalArrangement = Arrangement.Center
    ) {
        // Basic button
        Button(onClick = { 
            println("Button clicked!")
        }) {
            Text("Tap Me")
        }
        
        Spacer(modifier = Modifier.height(16.dp))
        
        // Custom styled button
        Button(
            onClick = { handleButtonClick() },
            colors = ButtonDefaults.buttonColors(
                containerColor = MaterialTheme.colorScheme.secondary
            ),
            modifier = Modifier
                .fillMaxWidth()
                .padding(horizontal = 32.dp)
        ) {
            Text("Custom Button")
        }
    }
}

fun handleButtonClick() {
    println("Custom button was clicked!")
}
```
{% endif %}

{% if visitor.isSet == false %}
<a href="https://support-examples.gitbook.io/conditions/?visitor.example_android=android" class="button primary" data-icon="android">Android</a> <a href="https://support-examples.gitbook.io/conditions/?visitor.example_android=apple" class="button secondary" data-icon="apple">Apple</a> <a href="https://support-examples.gitbook.io/conditions/?visitor.example_android=ubuntu" class="button secondary" data-icon="ubuntu">Ubuntu</a>

Kotlin Code:

```kotlin

import androidx.compose.foundation.layout.*
import androidx.compose.material3.*
import androidx.compose.runtime.Composable
import androidx.compose.ui.Alignment
import androidx.compose.ui.Modifier
import androidx.compose.ui.unit.dp

@Composable
fun ButtonExample() {
    Column(
        modifier = Modifier.fillMaxSize(),
        horizontalAlignment = Alignment.CenterHorizontally,
        verticalArrangement = Arrangement.Center
    ) {
        // Basic button
        Button(onClick = { 
            println("Button clicked!")
        }) {
            Text("Tap Me")
        }
        
        Spacer(modifier = Modifier.height(16.dp))
        
        // Custom styled button
        Button(
            onClick = { handleButtonClick() },
            colors = ButtonDefaults.buttonColors(
                containerColor = MaterialTheme.colorScheme.secondary
            ),
            modifier = Modifier
                .fillMaxWidth()
                .padding(horizontal = 32.dp)
        ) {
            Text("Custom Button")
        }
    }
}

fun handleButtonClick() {
    println("Custom button was clicked!")
}
```
{% endif %}

{% if visitor.claims.unsigned.example_android == "apple" %}
<a href="https://support-examples.gitbook.io/conditions/?visitor.example_android=android" class="button secondary" data-icon="android">Android</a> <a href="https://support-examples.gitbook.io/conditions/?visitor.example_android=apple" class="button primary" data-icon="apple">Apple</a> <a href="https://support-examples.gitbook.io/conditions/?visitor.example_android=ubuntu" class="button secondary" data-icon="ubuntu">Ubuntu</a>&#x20;



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
{% endif %}

{% if visitor.claims.unsigned.example_android == "ubuntu" %}
<a href="https://support-examples.gitbook.io/conditions/?visitor.example_android=android" class="button secondary" data-icon="android">Android</a> <a href="https://support-examples.gitbook.io/conditions/?visitor.example_android=apple" class="button secondary" data-icon="apple">Apple</a>  <a href="https://support-examples.gitbook.io/conditions/?visitor.example_android=ubuntu" class="button primary" data-icon="ubuntu">Ubuntu</a>



Code:

```c
#include <gtk/gtk.h>

static void button_clicked(GtkWidget *widget, gpointer data) {
    g_print("Ubuntu button clicked!\n");
}

int main(int argc, char *argv[]) {
    GtkWidget *window;
    GtkWidget *button;
    
    gtk_init(&argc, &argv);
    
    window = gtk_window_new(GTK_WINDOW_TOPLEVEL);
    gtk_window_set_title(GTK_WINDOW(window), "Ubuntu Button");
    gtk_window_set_default_size(GTK_WINDOW(window), 300, 200);
    
    button = gtk_button_new_with_label("Ubuntu Button");
    g_signal_connect(button, "clicked", G_CALLBACK(button_clicked), NULL);
    
    gtk_container_add(GTK_CONTAINER(window), button);
    gtk_widget_show_all(window);
    
    g_signal_connect(window, "destroy", G_CALLBACK(gtk_main_quit), NULL);
    
    gtk_main();
    return 0;
}
```
{% endif %}


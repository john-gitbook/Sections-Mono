---
title: Icons
---

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

# MODUL-
PRAKTIKUM
import tkinter as tk

def on_submit():
    name = entry.get()
    output_label.config(text=f"Halo {name}")

# Membuat window utama
root = tk.Tk()
root.title("GUI Praktikum")
root.geometry("300x150")

# Membuat input text
entry = tk.Entry(root, width=30)
entry.pack(pady=10)

# Membuat tombol submit
submit_button = tk.Button(root, text="Submit/Kirim", command=on_submit)
submit_button.pack(pady=5)

# Membuat label output
output_label = tk.Label(root, text="", fg="blue")
output_label.pack(pady=10)

# Menjalankan aplikasi
root.mainloop()

import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

df = pd.DataFrame({
    "order_id": list(range(101, 116)),
    "date": ["2026-10-01", "2026-10-01", "2026-10-02", "2026-10-02", "2026-10-03",
             "2026-10-03", "2026-10-04", "2026-10-04", "2026-10-05", "2026-10-05",
             "2026-10-06", "2026-10-06", "2026-10-07", "2026-10-07", "2026-10-08"],
    "customer": ["Aarav", "Diya", "Kabir", "Sneha", "Aarav", "Rohan", "Diya", "Kabir",
                 "Sneha", "Rohan", "Aarav", "Diya", "Kabir", "Sneha", "Rohan"],
    "city": ["Mumbai", "Delhi", "Bengaluru", "Mumbai", "Mumbai", "Delhi", "Delhi", "Bengaluru",
             "Mumbai", "Delhi", "Mumbai", "Delhi", "Bengaluru", "Mumbai", "Delhi"],
    "cuisine": ["Biryani", "Pizza", "South Indian", "Chinese", "Pizza", "Biryani", "Chinese",
                "Biryani", "Pizza", "South Indian", "Chinese", "Biryani", "Pizza",
                "South Indian", "Chinese"],
    "amount": [320, 450, 180, 260, 520, 300, 240, 350, 480, 150, 280, 340, 410, 200, 230],
    "rating": [4.5, 4.0, 4.6, 3.8, 4.2, 4.7, 3.9, 4.4, 4.1, 4.8, 3.7, 4.6, 4.3, 4.5, 4.0],
    "delivery_min": [35, 28, 22, 30, 32, 40, 25, 38, 27, 18, 33, 36, 29, 20, 26]
})

print(df.head())
print("https://github.com/sakhader88-cloud/Food-Orders/blob/main/food_orders.csv")
import pandas as pd
url = "https://raw.githubusercontent.com/sakhader88-cloud/Food-Orders/refs/heads/main/food_orders.csv"
df = pd.read_csv(url)
print(df)
df.head(2)
df.info()
df.to_csv("food_orders.csv", index=False)

# EDA
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

auto = pd.read_csv('/content/test-2.csv')

print(auto.head())
auto.isnull().sum()
sns.heatmap(auto.isnull(),cbar=False,cmap='viridis')

# matplotlid-assignment

ble for Iris dataset, but let's create simple line plot)
sns.set()
plt.figure(figsize=(8, 6))
plt.plot(df['sepal length(cm)'], label='Sepal Length')
plt.title('Sepal Length Trend')
plt.xlabel('Index')
plt.ylabel('Sepal Length (cm)')
plt.legend()
plt.show()

# Bar chart
plt.figure(figsize=(8, 6))
sns.barplot(x='species', y='sepal length (cm)', data=df)
plt.title('Average Sepal Length per Species')
plt.xlabel('Species')
plt.ylabel('Sepal Length(cm)')
plt.show()

# Histogram
plt.figure(figsize=(8, 6))
sns.histplot(df['sepal length(cm), kde=True'])
plt.title('Distributio of Sepal Length')
plt.xlabel('Sepal Length(cm)')
plt.ylabel('Count')
plt.show()

# Scatter plot
plt.figure(figsize=(8, 6))
sns.scatterplot(x='sepal length(cm)', y='petal length(cm)', hue='species', data=df)
plt.title('Relationship between Sepal and Petal Length')
plt.xlabel('Sepal Length(cm)')
plt.ylabel('Petal Length(cm)')
plt.legend()
plt.show

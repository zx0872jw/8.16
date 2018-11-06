# 8.16
# Put def average_weight(weights):  ... on line 3

    avg_weight = sum(weights)
    avg_weight = avg_weight / len(weights)
    print("\nAverage weight: %0.2f"  % avg_weight)

def max_weight(weights):
    max_weight = max(weights)
    print("Max weight: %0.2f" % max_weight)
    
def weight_location(weights):
    index = int(input("\nEnter a list index (1 - 4):\n"))
    lbs_to_kilo = weights[index-1] / 2.2
    print("Weight in pounds: %0.2f" % weights[index-1])
    print("Weight in kilograms: %0.2f\n" % lbs_to_kilo)

def sort_weights(weights):
    weights.sort()
    print("Sorted list:", weights)

def main():
    weight1 = float(input("Enter weight 1:\n"))
    weight2 = float(input("Enter weight 2:\n"))
    weight3 = float(input("Enter weight 3:\n"))
    weight4 = float(input("Enter weight 4:\n"))

    weights = []
    weights.append(weight1)
    weights.append(weight2)
    weights.append(weight3)
    weights.append(weight4)
    print("Weights:", weights)

    average_weight(weights)
    
    max_weight(weights)
    
    weight_location(weights)
    
    sort_weights(weights)
    
main()

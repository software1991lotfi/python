# python
bubblesort the python
def bubbleSort(asc):
	n = len(asc)
	swapped = False
	for i in range(n-1):
		for j in range(0, n-i-1):
      
			if asc[j] > asc[j + 1]:
				swapped = True
				asc[j], asc[j + 1] = asc[j + 1], asc[j]
		
		if not swapped:
			return
asc = [64, 34, 25, 12, 22, 11, 90]

bubbleSort(asc)

print("Sorted asc is:")
for i in range(len(asc)):
	print("% d" % asc[i], end=" ")

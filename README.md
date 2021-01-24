# BUBBLE-SORT

# Complexity Analysis

# Time Complexity of Bubble sort

Best case scenario: The best case scenario occurs when the array is already sorted. In this case, no swapping will happen in the first iteration (The swapped variable will be false). So, when this happens, we break from the loop after the very first iteration. Hence, time complexity in the best case scenario is O(n) because it has to traverse through all the elements once.

Worst case and Average case scenario: In Bubble Sort, n-1 comparisons are done in the 1st pass, n-2 in 2nd pass, n-3 in 3rd pass and so on. So, the total number of comparisons will be:
Sum = (n-1) + (n-2) + (n-3) + ..... + 3 + 2 + 1 
Sum = n(n-1)/2
Hence, the time complexity is of the order n2 or O(n2).

# Space Complexity of Bubble sort
The space complexity for the algorithm is O(1), because only a single additional memory space is required i.e. for temporary variable used for swapping.

# Pseudocode of Bubble Sort Algorithm

bubbleSort( Arr[], totat_elements)
   
   for i = 0 to total_elements - 1 do:
      swapped = false
		
      for j = 0 to total_elements - i - 2 do:
      
         /* compare the adjacent elements */   
         if Arr[j] > Arr[j+1] then
            /* swap them */
            swap(Arr[j], Arr[j+1])		 
            swapped = true
         end if
         
      end for
      
      /*if no number was swapped that means 
      array is sorted now, break the loop.*/
      
      if(not swapped) then
         break
      end if
      
   end for
   
end

# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.

Answer: To verify the claim of a O(n) comparison based sorting algorithm we would experimentally test its runtime by sorting lists of varying sizes and plotting the runtime against input size to see if it scales linearly if that makes sense. But theoretical analysis suggests that such a claim contradicts the known (nlogn) lower bound for comparison-based sorting algorithms, derived from the number of comparisons required to distinguish n! permutations. If the algorithm achieves O(n) it must either leverage additional input assumptions or use non comparison based techniques, like those in radix or bucket sort. Experiments can provide evidence but theoretical constraints make the claim seem like it is likely false unless the algorithm deviates.

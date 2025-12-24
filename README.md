# Python_Daily_Practice
Daily Python practice to build strong fundamentals, problem-solving skills, and data science readiness through consistent coding.
Foundation in:
-Python Fundamentals
-Data Structures
-Data Science
-Interview Level Problem Solvings

Started:24th December,2025
Goal:One Meaningful commit every day

def pair_sum(nums, target):
    left, right = 0, len(nums) - 1
    
    while left < right:
        curr_sum = nums[left] + nums[right]
        
        if curr_sum == target:
            return True
        
        if curr_sum < target:
            left += 1
        else:
            right -= 1
    
    return False

# Example
print(pair_sum([1, 2, 3, 4, 6], 7))  # True

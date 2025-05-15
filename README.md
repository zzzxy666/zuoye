def thirdMax(nums):# 定义函数thirdMax，找出数组中第三大的数，如果不存在则返回最大的数
   new_nums = sorted(list(set(nums)), reverse = True) # 使用set函数对数组nums去重，然后将其转换为列表并从大到小排序，得到去重且排序后的数组new_nums
  if len(new_nums) >= 3: # 使用set函数对数组nums去重，然后将其转换为列表并从大到小排序，得到去重且排序后的数组new_nums
        # 如果满足条件，说明存在第三大的数，返回该数
        return new_nums[2]
    else:
        # 如果不满足条件，说明不存在第三大的数，返回数组中最大的数
        return new_nums[0]

# 定义测试数组nums
nums = [3, 2, 1]
# 调用函数thirdMax并打印结果
print(thirdMax(nums))




def thirdMax(nums): # 定义一个函数thirdMax，用来找出数组中第三大的数，如果不存在第三大的数，就返回最大的数
   
    new_nums = sorted(set(nums), reverse=True) # 对输入的数组nums进行去重操作，然后将去重后的结果按从大到小的顺序排序，存到new_nums这个列表里
    # 判断new_nums这个列表的长度
    if len(new_nums) >= 3:
        # 如果长度大于等于3，就返回列表中索引为2的元素，也就是第三大的数
        return new_nums[2]
    else:
        # 如果长度小于3，就返回列表中的第一个元素，也就是最大的数
        return new_nums[0]

# 定义一个测试用的数组nums
nums = [1, 2]
# 调用thirdMax函数，把结果存到result变量里
result = thirdMax(nums)
# 打印出result的值
print(result)


# 定义一个数组nums
nums = [2, 2, 3, 1]
# 去除数组中的重复元素，得到新数组new_nums
new_nums = list(set(nums))
# 对new_nums从大到小排序
new_nums.sort(reverse=True)
# 判断新数组的长度是否大于等于3
if len(new_nums) >= 3:
    # 如果满足条件，第三大的数是索引为2的元素
    result = new_nums[2]
else:
    # 否则，返回最大的数（索引为0的元素）
这是我的作业

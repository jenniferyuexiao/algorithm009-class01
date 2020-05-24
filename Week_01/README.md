学习笔记

1. 可以训练。刷题切忌刷一遍，刷五遍，看discussion

2. 自顶向下的编程方法：

public boolean isPalindrom (String s) {

  //1. Filter out number & char
  //2. Reverse and Compare
  
  String filteredString = filterNonNumberAndChar(s);
  
  String reveredString = reverseString(filteredString);
  
  return reveredString.equalsIgnoreCase(filteredSting);
}

private String filterNonNumberAndChar (String s) {
  return s.replaceAll("[^A-Za-z0-9]", "");
}

private String reverseString(String filteredString) {
  return new StringBuilder(s).reverse().toString();
}

3.解题思路： 找最近的重复子问题
计算机只能执行“if else” 和 recursion，所以要找到问题的重复性

public int fib(int N) {
  if (N <= 1) {
    return N;
  }
  return fib(N-1) + fib(N-2);
}

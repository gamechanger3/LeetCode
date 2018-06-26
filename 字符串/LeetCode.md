# LeetCode

## 字符串

344.请编写一个函数，其功能是将输入的字符串反转过来。 

```java
class Solution {
    public String reverseString(String s) {
        StringBuilder str = new StringBuilder("");
        for(int i = 0; i < s.length(); i++){
            str.append(s.charAt(s.length()- i - 1));
        }
        return str.toString();
        
    }
}
```

```python
class Solution:
    def reverseString(self, s):
        """
        :type s: str
        :rtype: str
        """
        a = ''
        for i in range(len(s)):
            a += s[len(s)- 1- i]  
        return a
            
```



```java
class Solution {
public:
    String reverseString(String s) {
        int left = 0, right = s.length() - 1;
        while (left < right) {
            char t = s.charAt(left);
            s.charAt(left++) = s.charAt(right);
            s.charAt(right--) = t;
        }
        return s;
    }
}

int left = 0, right = s.size() - 1;
while(left < right){
    char t = s.charAt(left);
    s.charAt(left) = s.charAt(right);
    s.charAt(right) = t;
    left++;
    right--
}
```

swap函数

```java
class Solution{
    public :
    String reverseString(String s){
        int left = 0, right = s.length() - 1;
        while(left < right){
            swap(s.charAt(left++), s.charAt(right--));
        }
        return s;
    }
}
```


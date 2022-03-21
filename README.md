# 日常刷题的小知识

## set::find()

  标准定义：
```
  const_iterator find (const value_type& val) const;
  iterator       find (const value_type& val);
```
  定义一个set<string>，如果想要遍历一个string中的每一个元素，看是否在set中，由于string[]方法返回的是char类型，下面的执行是错误的：
```
  string a = "abcd";
  set<string> s;
  s.insert("a");
  s.find(a[0]);
```
  如果非要这么执行，需要将string[]的结果转换为string才可以

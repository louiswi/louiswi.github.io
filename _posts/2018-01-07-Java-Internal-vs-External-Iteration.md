---
layout: post
title: Be Yourself
date: 2018-01-07 13:11:11.000000000 +08:00
tags: Louiswi Github
---

##### External Iteration

This Iteration is called by Java builtin functions.

```
public void testInternalIteration() {


    List<String> list1 = Arrays.asList("aa", "bb", "cc");

    list1.forEach(System.out::println);

    Map<String, String> map1 = new HashMap<>();
    map1.put("1", "aa");
    map1.put("2", "bb");
    map1.put("3", "cc");

    map1.forEach((k, v) -> {
        System.out.println(k);
        System.out.println(v);
    });

}
```

##### Internal iteration

This Iteration is called by object method.

```
    public void testExternalIteraton() {

        List<String> list1 = Arrays.asList("aa", "bb", "cc");

        for (String i : list1) {
            System.out.println(i);
        }

        Map<String, String> map1 = new HashMap<>();
        map1.put("1", "aa");
        map1.put("2", "bb");
        map1.put("3", "cc");

        for (Map.Entry<String, String> entry : map1.entrySet()){
            System.out.println(entry.getKey());
            System.out.println(entry.getValue());
        }

    }
```
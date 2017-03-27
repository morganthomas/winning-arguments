## Natural numbers

A natural number is a non-negative, non-fractional number. In other words, the natural numbers are 0, 1, 2, 3, 4, and so forth. 

An **expression** (of natural numbers) is any piece of writing which can be produced by the following rules:

 * Variable names are expressions: *a*, *b*, *c*, ...
 * 0 and 1 are expressions.
 * If **a** and **b** are expressions, then:
   * (**a** + **b**) is an expression.
   * (**a** * **b**) is an expression.

The following are examples of expressions:

 * *a*
 * 0
 * 1
 * (*a* + 0)
 * (1 + *b*)
 * (1 + (1 + *b*))
 * (1 + (1 + (1 + 0)))
 * (*a* * 0)
 * (1 * *a*)
 * ((1 + (1 + 0)) * (*b* + *c*))

A **statement** (about natural numbers) is any piece of writing which can be produced by the following rules.

1. If **a** and **b** are expressions, then:
    * (**a** < **b**) is a statement.
    * (**a** = **b**) is a statement.
2. If **A** is a statement, then (not **A**) is a statement.
3. If **A** is a statement and **B** is a statement, then:
    * (if **A** then **B**) is a statement.
    * (**A** and **B**) is a statement.
    * (**A** or **B**) is a statement.
4. If **A** is a statement and **a** is a variable name, then:
    * (for all **a**, **A**) is a statement.
    * (for some **a**, **A**) is a statement.

Notice that except for the first rule, these are all rules of statement formation in first-order logic. The first rule essentially says that the object literals of the language are expressions (of natural numbers), and that the available copulas are < and =. Predicates and the "is" connective are not part of our language for talking about natural numbers. Here are some examples of statements about natural numbers, some true and some false:

 * (0 < 1)
 * (0 = 0)
 * (1 = 0)
 * ((1 + (1 + 1)) = ((1 + 1) + 1))
 * (for all *a*, (for some *b*, ((a+1)=b)))
 * (for all *a*, (for all *b*, (if (a < b) then ((a + 1) < (b + 1)))))
 * (for some *a*, (for some *b*, (for some *c*, ((a > 0) and (b > 0) and (c > 0) and (((a * (a * a)) + (b * (b * b))) = (c * (c * c)))))))

Now we know what a statement about natural numbers is. We have promised to argue that every statement about natural numbers is either true or false. To argue this, clearly we need to know what it means for a statement about natural numbers to be true (or false). Fortunately, there is a conventional definition of truth for statements about natural numbers, which is simple to give. I believe this style of truth definition is originally due to Tarski.

The definition of truth is context-sensitive. Recall that a context 

 * 

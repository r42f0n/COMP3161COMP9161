java c
COMP3161/COMP9161 
Concepts of Programming Languages 
Sample Exam 
Session   2   2011 
Question 1 [25 Marks] 
Consider   the   following   inductive   deﬁnition   of evaluation rules   for   a restricted   form   of boolean   expres-   sions.
Boolean expressions: 

Evaluation rules: 


A) [7 marks] 
Give the derivation of the evaluation for the following expression:
•      and(not(false); and(true;   not(true)))
B) [7 marks] 
Are   the   rules   unambiguous?   If   so, brieﬂy   explain   why.   If   not, give   an   example   expression   for   which the set of   rules allow more   than   a   single   derivation.
C) [11 marks] 
The rules listed above give a small step   semantics.   List the   inference rules   which   specify   an   equiv-   alent big step   semantics.
Question 2 [25 Marks] 
A) [10 marks] In   the   lecture,   we   discussed   the   E-machine   as   an   example   of   an   abstract   machine   which   handles   value bindings explicitly by maintaining a value environment.   One of the possible return values   of   the E-machine are function closures.
i)    What   is   a   function   closure?
ii)    Give an example of an expression   whose   evaluation   in   the   E-machine   requires   the   creation   of   a   closure.
B) [15 marks] We   discussed   two   distinct   methods   to   handle   exceptions:   the   ﬁrst   method   required   that,   when   an   exception is thrown, the evaluation unrolls   the   stack   until   the   matching   catch-expression   is   found.   The   second method made it possible   to   directly jump to   the   matching   catch-expression.    Describe   the second   method:
i)    What   are   the   components   of   the   state   of   the   abstract   machine?
ii)    How does the state of the machine change when a   catch-expression is evaluated?
iii)    How does the state of the machine change when a   raise-expression is evaluated?
For   (ii) and   (iii),代 写COMP3161/COMP9161 Concepts of Programming Languages Session 2 2011Java
代做程序编程语言 you   do   not   have   to   give   the   exact   transition   rule   —   it   is   sufﬁcient   to   describe   how the state   is   affected.
Question 3 [25 Marks] 
A) [6 marks] 
For   each   of the   following   three   pairs   of type   expressions   determine   whether   the   pair   has   a   most   general   uniﬁer?   If   so, please   provide   it.
i)      (a   , b)    →      (b   , a) and   (int   ,   c) → (c   ,    c)
ii)      a → (a   , a) and   (b   , b) → b
iii)      int → int   and float → int
B) [9 marks] 
Give the principal type of the following (polymorphic) MinHs expressions:
i)      Inr(Inl(True))
ii)      letfun      f         (x)      is      fst         (snd         (x));
iii)      letfun      g         (x)      is
case      x      of    Inl(a)      ->      a
Inr(b)      ->      b
end
end
C) [10 marks] 
Consider the following MinHs types:
•   8a.8b.(a * b   →   c)   →   (a   →   b   →   c)
•   8a.8b.(a   →   b)   →   (b   →   a)
•   8a.8b.8c.(a   →   b)   →   (b   →   c)   →   (c   →   a)
•   8a.()   →   a
•   8a.a   →   ()
For which of these types exist terminating MinHs functions?
Question 4 [25 Marks] 
A) [10 marks] 
Progress and preservation are central concepts for strongly typed   languages.
i)    Give   the   deﬁnition   of progress   and   of   preservation   in   the   context   of   a   strongly   typed   language. 
ii)    The presence   of partial   functions   can be problematic   with respect   to   progress.    Describe how   they can be handled in a strongly typed language such that both progress and   preservation still   hold.
B) [5 marks] 
Give   an   example   each   for   a   type   constructor   which   is   covariant   and   a   type   constructor   which   is   contravariant in at least one of its argument positions.
C) [10 marks] 
Java’s   array   type   is   covariant.   Why   is   this   problematic?

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com

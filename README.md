# Strong induction

[StrongInduction.v](StrongInduction.v) proves the principle of strong induction
over natural numbers:

```coq
Theorem strong_induction : forall P : nat -> Prop,
  (forall m : nat, (forall n : nat, n < m -> P n) -> P m) ->
  forall n : nat, P n.
```

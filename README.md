# splitwise

Description-
A C++ program to minimize the total number of transactions among peers, who owe money to each other. Implemented an algorithm to minimize the total number of transactions using Maxheap.

Algorithm-
1. Compute the net amount for every person. The net amount for person āiā can be computed by subtracting sum of all debts from sum of all credits.
2. Find the two persons that are maximum creditor and maximum debtor. Let the maximum amount to be credited maximum creditor be maxCredit and maximum          amount to be debited from maximum debtor be maxDebit. Let the maximum debtor be Pd and maximum creditor be Pc.
3. Find the minimum of maxDebit and maxCredit. Let minimum of two be x. Debit āxā from Pd and credit this amount to Pc
4. If x is equal to maxCredit, then remove Pc from set of persons and recur for remaining (n-1) persons.
5. If x is equal to maxDebit, then remove Pd from set of persons and recur for remaining (n-1) persons.

![Screenshot from 2022-09-24 11-26-58](https://user-images.githubusercontent.com/42449449/192082957-954ebf25-20ec-41c3-835c-c88cf6667836.png)

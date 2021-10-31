# Reading and writing a State Variable

```
contract SimpleStorage {
    // State variable to store a number
    uint public num;

    // You need to send a transaction to write to a state variable.
    function set(uint _num) public {
        num = _num;
    }

    // You can read from a state variable without sending a transaction.
    function get() public view returns (uint) {
        return num;
    }
}
```

We saw earlier saw that each function call is a new transaction. Every transaction has a transaction fees.
To write or update a state variable you need to send a transaction & pay the fees.

On the other hand, you can read state variables, for free, without any transaction fee.

```
run testcases 04.sh
```
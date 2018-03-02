# X-Team 23 Style Guide

Make codes that can get A's.

## Naming conventions

As long as it is easy to understand, the name should no be ambiugous.
### Examples
* interfaces
* classes
* exception types
* fields
* methods
* parameters
* local variables
* instance constants
* class constants

## Commenting style for public and private members of a class or interface:

As long as it is understandbale, then it is ok.

### Examples

* classes
* fields
* constructors
* methods
* coding style (brackets, horizontal, and vertical spacing) for:
  * if statements
  * switch statement
  * while loops
  * for loops
  * enhanced for loops  
*///////////////////////////////////////////////////////////////////////////////  
// assignment name: p1 PQ  
// Author: Tianyuan(Rainer) Yuan  
// Email : tyuan22@wisc.edu  
// due date: Jan 5th 2018  
// CS Login: tyuan22  
// Credits: none  
// known bugs: none  
//////////////////////////////////////////////////////////////////////////////  
/**
 * Series of test for the maxPq constructed
 * 
 * @author yuantianyuan
 */
import java.util.Arrays;
import java.util.Random;

public class TestMaxPQ {

    /**
     * main method that run the tests
     * 
     * @param args print our string
     */
    public static void main(String[] args) {
        test1_isEmpty();
        test2_getMax_Exception();
        test3_removeMax_Exception();
        test4_insert_remove_1();
        test5_insert_many_remove_1();
        test6_dups_allowed();
        test7_big_data();
        test8_size();
    }

    /**
     * test1 tests weather the isEmpty() works properly
     */
    public static void test1_isEmpty() {
        PriorityQueueADT<Integer> pq = new MaxPQ<Integer>();
        Boolean passed = pq.isEmpty();
        if (passed) {
            System.out.println("test1_isEmpty passed");
        } else {
            System.out.println(
                            "test1_isEmpty failed: returned false instead of true when the PQ was just constructed.");
        }

    }

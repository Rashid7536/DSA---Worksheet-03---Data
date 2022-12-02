/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package com.mycompany.mavenproject1;
import java.util.Queue;
/**
 *
 * @author Rashid
 */
// Java program to remove elements
// from a Queue

import java.util.*;

public class NewClass1 {

	public static void main(String args[])
	{
		Queue<Integer> Que = new PriorityQueue<>();
                Random r = new Random();
                
                
		 //============STAGE 01===============//
                for(int i=0 ;i<=2000;i++){
                    
                    long inTime = System.nanoTime(); //using System library
                    //take the system time at this point
                    //create random numbers, since it
                    //will create negative numbers, a bound has been created,
                    //which means it can generate numebrs form 0-50000 and equate to ele
                    //which will be sent to the function
                    Que.add(r.nextInt(5000000));
                    long offTime = System.nanoTime(); // take the system time
                    //at this point
                    long totalTime = offTime - inTime; // calculate the time difference
                   
                    //System.out.println(totalTime); //record the time to the output
                
                }
                
                
                //============STAGE 02===============//
                for(int i=0 ;i<=18000;i++){
                    
                    long inTime = System.nanoTime(); //using System library
                    //take the system time at this point
                    //create random numbers, since it
                    //will create negative numbers, a bound has been created,
                    //which means it can generate numebrs form 0-50000 and equate to ele
                    //which will be sent to the function
                    Que.add(r.nextInt(50000000));
                    Que.add(r.nextInt(50000000));
                    Que.remove();
                    long offTime = System.nanoTime(); // take the system time
                    //at this point
                    long totalTime = offTime - inTime; // calculate the time difference
                   
                    //System.out.println(totalTime); //record the time to the output
                }
                
                
                //============STAGE 03===============//
                    for(int i=0 ;i<=20000;i++){
                    
                    long inTime = System.nanoTime(); //using System library
                    //take the system time at this point
                    //create random numbers, since it
                    //will create negative numbers, a bound has been created,
                    //which means it can generate numebrs form 0-50000 and equate to ele
                    //which will be sent to the function
                    
                    Que.remove();
                    long offTime = System.nanoTime(); // take the system time
                    //at this point
                    long totalTime = offTime - inTime; // calculate the time difference
                   
                    System.out.println(totalTime); //record the time to the output
                    }
                    
                    /* 
                    //============ STAGE - isFULL===============//
                    for(int i=0 ;i<=20000;i++){
                    
                    long inTime = System.nanoTime(); //using System library
                    //take the system time at this point
                    //create random numbers, since it
                    //will create negative numbers, a bound has been created,
                    //which means it can generate numebrs form 0-50000 and equate to ele
                    //which will be sent to the function
                    Que.add(r.nextInt(500000000));
                    Que.size();
                    
                    long offTime = System.nanoTime(); // take the system time
                    //at this point
                    long totalTime = offTime - inTime; // calculate the time difference
                   
                    System.out.println(totalTime); //record the time to the output
                    }
                    
                    //============ STAGE - isEmpty===============//
                    for(int i=0 ;i<=20000;i++){
                    
                    long inTime = System.nanoTime(); //using System library
                    //take the system time at this point
                    //create random numbers, since it
                    //will create negative numbers, a bound has been created,
                    //which means it can generate numebrs form 0-50000 and equate to ele
                    //which will be sent to the function
                    Que.remove();
                        if(Que.isEmpty()){
                            break;
                        }
                    long offTime = System.nanoTime(); // take the system time
                    //at this point
                    long totalTime = offTime - inTime; // calculate the time difference
                   
                    //System.out.println(totalTime); //record the time to the output
                    }
                        */
                    
	}
}


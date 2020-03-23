---
layout: post
title:      "Arrays and Data Sets"
date:       2020-03-23 18:48:04 -0400
permalink:  arrays_and_data_sets
---


Data sets are foundational to computer programming. They allow us to store and use data in useful ways. An example of a data set is a string. It stores text between apostrophes.
 
                     string=”I need money”
                     
										 string_1=”Hello World”

Another type of data set is an array. It stores texts and integers. They are lists of information inside brackets.
 
                     array=[10, “Eleven”, 12, “Twelve”, 13]
 
A major feature of arrays is they make information useful and acccessible through different methods and iteration.
Methods are commands that pulls individual data from an array. We use the Information to build programs.

* First pulls the first element from an array, and last gives us the last element.

                       [10, “Eleven”, 12, “Twelve”, 13].first=>10
                     
										   [10, “Eleven”, 12, “Twelve”, 13] .last=>13

* We extract the middle numbers through indexing. When we use indexes, the first number starts with zero. Then we
   count from there
.
                        [10,"Eleven",12,"Twelve", 13][0]=>10
                     
										    [10,"Eleven",12,"Twelve", 13][1]=>”Eleven”
                     
   										  [10,"Eleven",12,"Twelve", 13][2]=>12

* Push, insert, unshift, and shovel(<<) adds elements to an array.

                        [10,"Eleven",12,"Twelve", 13].push(14)
                         =>[10,"Eleven",12,"Twelve", 13, 14]
                       
											  [10,"Eleven",12,"Twelve", 13].insert(3,14)
                         => [10,"Eleven",12, 14, "Twelve", 13]
                       
											  [10,"Eleven",12,"Twelve", 13].unshift(9)
                        =>[9,10,"Eleven",12,"Twelve", 13]
                       
											 [10,"Eleven",12,"Twelve", 13]<<14
                        =>[10, "Eleven", 12, "Twelve", 13, 14]

* Pop, shift, delete, and delete_at removes elements from an array.

                      arr.pop=>[10,"Eleven",12,"Twelve"]
                     
		 								  arr.shift=>["Eleven",12,"Twelve", 13]
                     
			 							  arr.delete(12)=>[10,"Eleven",12,"Twelve", 13]
                      
										  arr,delete_at(2)=>[10, "Eleven", 13]


* Size, length, and count gives us a number of elements in an array.

                     arr=[10,"Eleven",12,"Twelve", 13]
                     
										         arr.size=>4
                             arr.length=>4
                             arr.count=>4

Iteration helps us manipulate specific elements of an array through blocks. Examples of iteration may include:

                    array=[1,2,3,4,5]

* Each returns a list of elements from an array.

                array.each{|n| puts n}
                1
                2
                3
                4
                5             
                =>[1,2,3,4,5]

* Select returns a new array based on a set of conditions. Detect returns the first value based on those conditions.

              array.select{|n| n<3}
               =>[1,2]

              array.detect{|n| n<3}
               =>1
 
* Collect and map returns a new array given certain conditions.
 
             array.map{|n| n*3}
              => [3, 6, 9, 12, 15]

* Any and include returns true if an element exists in an array.

             array.any(2)=>true
						 
             array.include?(2)=>true

* None checks if an element exists in an array. If it does, it returns false. Empty returns true if an array contains 
   no  elements. 

            array.none?(2)=>false

            array.empty?=>false

   Each returns false since the array contains the number two and has elements in it. 

Through iteration and different methods, arrays form a basic building block for programming. They enable us to build very complex programs and store huge amounts of data. 

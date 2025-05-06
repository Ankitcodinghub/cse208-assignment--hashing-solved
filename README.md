# cse208-assignment--hashing-solved
**TO GET THIS SOLUTION VISIT:** [CSE208 Assignment -Hashing Solved](https://www.ankitcodinghub.com/product/cse208-assignment-hashing-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;96901&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE208 Assignment -Hashing Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
1 Problem Specification

In this assignment, you have to implement a HashTable with the following requirements.

<ol>
<li>You have to implement insert, search, and delete operations on the hash table. The
length N of the hash table will be given as an input from console.
</li>
<li>The data will be kept as a (key, value) pair in the hash table. You need to in- sert randomly generated unique words of 7 character length (these words can be meaningful or meaningless) into the hash table. Therefore, you have to implement a random word generator. The words will be used as the “keys”, and the order of the incoming words will be used as the “value” (please see the example below). If your word generator generates duplicate words, you have to keep only one instance of those words.</li>
</ol>
2 Example

Suppose your word generator has generated the following 5 words.

ancient puzzled benefit ancient zigzags

The corresponding key-value pairs will be:

(ancient, 1) (puzzled, 2) (benefit, 3) (zigzags, 4)

You have to discard the second instance of the word “ancient” since it has already been included in the table.

1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
3 Hash Function

You have to use 2 standard hash functions (Hash1(k) and Hash2(k)) of your own, or from any good literature where you must try to avoid collisions as much as possible. We are expecting that 60% of the keys will have unique hash values (e.g., at least 60 unique hash values for 100 keys).

4 Collision Resolution

You need to implement the following three collision resolution methods.

<ol>
<li>Chaining Method

Place all the elements that hash to the same slot into a linked list. Slot j contains a pointer to the head of the list of all stored elements that hash to j ; if there are no such elements, slot j contains NULL.</li>
<li>Double Hashing

In case of Double hashing, use the hash function as follows.

doubleHash(k, ı) = (Hash(k) + i × auxHash(k)) % N

Here, Hash(k) is one of the hash functions described in Section 3. Note that you have to use both the Hash functions mentioned in Section 3 for report generation; see Section 5 for more details. Here, auxHash(k) is an auxiliary hash function. To keep things simple, you can use a simple hash function as the auxiliary hash function. The initial probe goes to position Table[Hash(k)], and successive probe positions are offset from previous positions by an amount auxHash(k), modulo N.
</li>
<li>Custom Probing

In case of Custom Probing, use a hash function of the form:

customHash(k, i) = (Hash(k) + C1 × i × auxHash(k) + C2 × i2) % N

Here, C1 and C2 are two auxiliary constants of your choice. The other details are same as the Double Hashing.
</li>
</ol>
</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
5 Report Generation

Generate 10000 seven character long unique words and insert them into the Hash Table. Mention the number of collisions in a tabular format using both the hash functions (e.g., Hash1 and Hash2). Among these 10000 generated words, randomly select 1000 words and search each of these selected words in the hash table. Report the average number of probes (i.e., number of times you access the hash table) required to search the words. Please report these results for both the Hash functions (Hash1 and Hash2). The report should be generated in the following tabular format.

</div>
</div>
<div class="layoutArea">
<div class="column">
Collision Resolution Hash1

Method No. of Collisions Avg. Probes Chaining Method

Double Hashing

Custom Probing

</div>
<div class="column">
Hash2 No. of Collisions

</div>
<div class="column">
Avg. Probes

</div>
</div>
<div class="layoutArea">
<div class="column">
Table 1: Performance of various techniques for collision resolution with two different hash functions.

Note that, you may be asked to run your program during evaluation to show that the output of your program closely resembles the reported values (it is okay if they do not match exactly).

</div>
</div>
<div class="layoutArea">
<div class="column">
6

1. 2. 3.

</div>
</div>
<div class="layoutArea">
<div class="column">
&nbsp;

</div>
</div>
</div>

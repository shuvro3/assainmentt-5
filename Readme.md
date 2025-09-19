1.What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

Ans:
getElementById: নির্দিষ্ট id দিয়ে একটি মাত্র element কে খুঁজে বের করে

getElementsByClassName :নির্দিষ্ট একটি class নামের আইডিকে খুঁজে বের করে 

querySelector :  class নামের first আইডিকে খুঁজে বের করে কিন্তু css সিলেক্টর হিসেবে দিতে হয়

querySelectorAll:  class নামের সকল আইডিকে খুঁজে বের করে কিন্তু css সিলেক্টর হিসেবে দিতে হয়



2.How do you create and insert a new element into the DOM?
    Ans:

        <body>
        <div id= "newText">  </div>

        <script>
            const notun = document.createElement('p')
            notun.innerText = 'hello my name is shuvro'

            const container = document.getElementById('newText')
            container.appendChild(notun)
        </script>

        </body>



3.What is Event Bubbling and how does it work?
    Ans:যখন কোন element trigger  করা হয় event প্রথমে সেই এলিমেন্টে ঘটে তারপর প্যারেন্ট এলিমেন্টে যায় তারপর আরেকটু উপরে এলিমেন্টে যায় এভাবে করতে করতে উপরের উঠতে থাকে যা একটি বুদবুদের মতো দেখায় যা জলের নিচে থেকে উপরে উঠছে এমন দেখায়



4.What is Event Delegation in JavaScript? Why is it useful?
Ans:child eleneeent এর জন্য আলাদা আলাদা event লিসেনার না দিয়ে তাদের প্যারেন্ট এলিমেন্ট এ একটাই ইভেন্ট লিসেনার বসানো আর ইভেন্ট Bubbling ব্যবহার করে child element-এর event handle করা।


5.What is the difference between preventDefault() and stopPropagation() methods?
Ans:
preventDefault():element er default কাজ বন্ধ করে দেয়। যেমন from tag এ পেজ রিলোড নেয় না

stopPropagation():ইভেন্টকে প্যারেন্ট element a যেতে দেয় না |

# inputTimestamp
Use this to find all inputs hidden or not and add the current time from the browser.
Very useful when you have know you will need a lot f time stamps in your project. Especially for forms.

# Instructions
1. Make sure jQuery is available to use in your project (v3.1.0 was used for this)
2. Include the time.js file in your project.
3. Give every input that needs a timestamp a suitable class name. e.g <input type='hidden' class='timestamp'/>
5. Call get_time() using the class used above for your inputs like below:


    $(document).ready(function(){
        //UPDATE TIME EVERY 5 SECONDS
        get_time('timestamp');
        setInterval(function(){
            get_time('timestamp');
        },5000);
    });

6. Adjust the time update as needed. 


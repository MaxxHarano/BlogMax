+++
title = 'Interview Log1'
date = 2024-05-11T02:00:56+08:00
draft = false
+++


# Interviews 
### with Max

---

I've been through a lot for the last few weeks.
More precisely, there has been a bunch of interviews in a row.
Here's a list for details:

1. Apr. 18 w/ ByteDance
1. Apr. 29 w/ 
1. May 6 w/ DingTalk
1. May 7 w/ HyperLink
2. May 9 w/ HelloBike
3. May 10 w/ Tencent

If you'd like to know how I feel about the speific interviewers :

<details>
    <summary>ByteDance</summary>
    Very gentle and patient with me. Guided me through the whole algo test (knowing I'm a **noob**).
</details>

<details>
    <summary>ByteDance</summary>
    Sounds like an aged gentleman, with course voice and fatherly manners.
</details>

<details>
    <summary>Dingtalk</summary>
    It might be that I was unable to connect for the first two times, which made this person sounds slightly  aggressive to me. Or that he's just a literal sociopath.
</details>

<details>
    <summary>HyperLink</summary>
    THE BEST interviewer so far. Calm and respectful. Feels easy to communicate with.
</details>

The thing is that, it took quite a while for some of these interviewers to respond or move on to the next question. 
<span style="color:gray">
I'm assuming they're just looking for questions on the Internet or somewhere else.
</sapn>

In the following section I'll be documenting the exact questions I've *personally* encountered during these interviews.

In order to avoid awkwardness, I'll provide IDEAL answers to some of questions, rather than my actual answers at the time. 

## Un_ ByteDance 
#### duration: 1 hr

1. Have you ever written codes with vannilla JS?

  Me: Yes.
1. How do you perceive the Frameworks used in Frontend develpoing

  Me: React uses components and ...
1. Why the frameworks provide better functionality?

  Me: They enable the developers to create frontend with programming thought process.  
1. **Virtual DOM** [^1]

   The Interviewer: what functionality does the Virtual DOM meliates?
  Me: ...(didn't know by the time)
1. Please describe the process of a HTTP request.

   Me: (Yapping about the network layers)
1. Have you ever captured packages or seen how a http request was sent?

    Me: We were assigned to use Wireshark in a course ... (???)
  The Interviewer: Wireshark works on the TCP layer. // digresses
1. What's **the difference between a GET and a POST request**? [^2]

  Me searching for answers: GET wraps params inside of the URL 

  The Interviewer: POST can also do that.

  Me: Yeah...(speechless)

  The Interviewer: What's the semantic difference between the two?

  Me: GET is used to fetch data, while POST is used to submit data. (I was searching for the answer) GET would be cached but POST would not.

  The Interviewer: Would there be a problem if POST was cached?

  (Me trippin' ...)

  Correct Answer:
  >
1. **What optimization do we see in HTTP 2.0 over 1.0?** [^3]
  (IDK)
  Correct Answer: 
  >
1. How does HTTPS ensures security?
  Me: End to end encryption and keys.
  Correct Answer:
  >
1.  What if the key was altered?
   
  Correct Answer:
  >

---
Moving on to the browser aspect.
Keywords: *Cookie, session*

1.  Describe how cookie works.

  Correct Answer:
  >
1.  Then what about sessions?
   
  Correct Answer:
  >
1.  Why is cookie less commonly used nowadays?
   
  Me: to enhance security??
1.  Explicate on the security of cookie.
   
2.  Are you familiar with any other authentication methods?
  Me: Hmm...
  Correct Answer:
  >

---
A practical css  question followed:

16. How do you make an element vertically and horizontally align to the center of a div.

  Me: Use align-items: center or justify-content.
  The Interviewer: Is there any other ways?
  <span style="color:gray">
  //Trying to make me say use Flex
  </span>
  Me: Maybe use Grid?

1. What novel features do you think HTML and CSS have?

  (Me trying to figure out what he meant.)
  The Interviewer: It came out in recent years and has great potential.

1. What sites do you use to learn Web dev?

  Me: w3school (OMFG...)
  The Interviewer: Have you ever checked out MDN web doc?
  Me; Yes.
  (Him realizing that I'm "problem-driven" in developing)

---
A very specific scenario was provided:

- How do you make sure a countdown page was accurate and sync with the server side.
  Me: Implement some synchronizing mechanism.
  The Interviewer: Can you explain further?

  The IDEAL answer:
  >

#### Coding test part

He basically provided a simple JS debounce question, which I had no clue back then.

## Deux_  
#### duration: 20 min

This one hits different.
And I love it.

- The latest React version has been updated to 19. Hooks are available only after v16. Can you describe the usage of the hook **useEffect**?
- When does useEffect performs an action?
  Me: when the dependencies changes.
- **Then what if you leave the dependency blank, as an empty array?** [^4]
  Correct Answer:
  >
- What if you don't fill anything there?
  > Him: If you don't fill the second param, the function would be carried out frequently. If you at least fill an empty array, the hook would take action when the component initializes. There are two stages of a component, Initialization and Updates.
- Which Hook should you use if you'd like to reference a DOM?
  Me: ? // I should have known better at that time.
  Him: To make the value not affected by the component renders.
  Obviously **useRef**...

---
Moving on to ES6 syntax.

- **Arrow Functions** What are the differences between arrow functions and normal functions?
  
  Correct Answer:
  >

- Why comes the arrow function?
  

- How do you listen to events in vanilla JS?
  (It was obvious but I...)

- Do you know about **event bubbling** and **event capturing**?
  [Geek explaination](https://www.geeksforgeeks.org/what-is-event-bubbling-and-event-capturing-in-javascript/)


## Trois_ DingTalk 
#### duration: 30 min

## Quatre_ HyperLink 
### duration: 40 min

This one also went hard with the React Routing...
First she asked about my project and then goes deep into it.
For the sake of practicality, I'll only provide the Ideal answers here.

1. How does create Route From Element implement its effect?
1. Can you explain the differences between creating Routes using *Hash* and using *History*?
1. What do you think of the ad/disadvantages when using these routing methods?
1. Tell me about the differences between Single page Multiple page Apps.
1. Explain JSX.
1. So how are JSX converted into HTML?
1. **Virtual DOM** [^1]
1. How does it reduces unneccessary renders? More precisely, how is the diff funtion carried out?
1. Why do browsers suggest you use T val when using the .map method?
  Me: (IDK)
  Her: it's about the GUI, you can take notice in console logs next time.
1. Do we only use hooks in React or can you also use classComponents? 
1. Why Hooks can only be used at top level of a component but not in loops?
1. What does **ref** do in components?
1. How do you create a Timer with useRef?
// And she actually wanted to ask a debounce question... omg



## Cinq_ HelloBike
### duration: 20 min
date: 05-11-2024

1. Do you have any cool function in your project?
   Me: no I only did the basics (trying to be honest)
2. How is HTTP2.0 better than 10.
3. **What is the use of passing an empty array as the second dependency of the useEffect Hook?**[^4]

## Six_ Tencent
### duration: 30 min

1. Do you have any cool function in your project?
   ...
2. How do you start a project then?

   Me: create react app (not knowing what he was trying to ask about)
3. I saw you used vite.

   Ok
4. Did you use ES6 or ES5?

    ES6
5. Where is the code stored?
   ( He setting me up...)
   
    in browser
6. ES6 cannot run in browser so how do you even do that?
   
   Emmm
7. So how to convert ES6 to ES5?

    Use tools like Babel

8. Have you used it?

    (Bitch do you even use it yourself...?)

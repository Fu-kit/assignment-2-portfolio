# assignment-2-portfolio
portfolio of week 6-12

Week 6

---What prompt(s) did you try?

"I got the following error, and I assume that... To what extent am I correct?"

Actual conversation;
-----------------------------------------------------------------------------
(Me)
I got the error;

NameError                                 Traceback (most recent call last)
/tmp/ipython-input-261853233.py in <cell line: 0>()
      9 
     10 ### A2. Add a new entry (your name)
---> 11 person["name"] = "Fuki"
     12 person["phone"] = "0433-987-654"
     13 

I assume that we firstly have to define person, instead of contact, if I use person.

(AI)

---

### 📘 Answer in English

Yes, exactly 👍
The error happens because **`person` was never defined**. You only created a dictionary called `contacts`.

If your goal is to **add yourself to the `contacts` dictionary**, you don’t need `person` at all. Just do:

```python
contacts["Fuki"] = "0433-987-654"
```

This way, `"Fuki"` is added as a **new key** in the `contacts` dictionary, with the phone number as its **value**.

After that, `contacts` will look like:

```python
{
    "Alice": "0400-123-456",
    "Bob": "0411-000-999",
    "Charlie": "0422-111-222",
    "Fuki": "0433-987-654"
}
```
(Answer in Japanese)
---
👉 Fuki, do you want me to also show you how to **update** a contact’s number (Part A3 of your worksheet) using the same style?

-----------------------------------------------------------------------------



---What did you change/fix from AI’s suggestion?

I changed (1) to (2).

(1)
for key, value in contacts.items():
    print(f"'{key}': '{value}',")

(2)
for key, value in contacts.items():
    print(f"{key}: {value}")

Outputs are like;

(1)
'Alice': '0400-123-456',
'Bob': '0411-000-000',
'Charlie': '0422-111-222',

(2)
Alice: 0400-123-456
Bob: 0411-000-000
Charlie: 0422-111-222

I would like to delete '' in output and asked human friednly code to my AI.
---One concept you want to practise (e.g., .items(), .get()).


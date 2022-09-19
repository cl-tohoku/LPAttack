# LPAttack: A Feasible Annotation Scheme for Capturing Logic Pattern of Attacks in Arguments

## Overview
LPAttack (Logic Pattern of Attack) is an annotation scheme that captures the common modes and complex rhetorical moves in attacks in arguments along with the implicit presuppositions and value judgments. This repository consists the corpus (logic patterns of attacks of 250 debates) annotated by the LPAttack scheme and the annotation guidelines.

![overview](https://github.com/cl-tohoku/LPAttack/blob/master/lpattack_example.jpg "overview")

## Corpus
We utilized the debates from the TYPIC dataset (Naito et al. 2022) for LPAttack annotation. Each debate consists an Initial argument, referred to as "PM Speech" (speech from Prime Minister) and a Counterargument, referred to as "LO Speech" (speech from Leader of Opposition). The debates are wriiten for 2 topics: `Death penalty should be abolished` and `Homework should be abolished`. 

In each of the topic folder, the `JSON` folder consists the data the `DRAWIO` folder consists the visual diagrams for the data (can be opened and seen using https://www.diagrams.net/).
The data in the .json files looks like below:

```
{
  "PM": "Hello everyone. Today's topic is \"Homework should be abolished\". We have two points: The first point is \"free time\" and the second point is \"decrease burden on teachers\". I will explain the first point of \"free time\". We believe that if homework were to be abolished, we could have more free time. As a result, we could do more of what we really wanted like club activities, hobbies, or playing with friends. In my case, I go to tennis club after class until 5:00 pm and then I go to cram school until 8:00 pm. After this full day, I arrive at my home around 8:40 pm to eat dinner and take a shower. At nearly 10:00 pm I start my homework. I have a lot of homework. As a result, I go to bed late at night at nearly 1:00 am in the morning and I don't have the opportunity to sleep for a long period of time. It is not healthy. Therefore, homework should be abolished. Thank you.",
  "LO": "They said that students will have more free time by abolishing homework. However, what students will do during free time is just playing games and chatting using SNS in most cases or just sleeping as they said. It is because human is lazy in nature. Doing hard thing is usually difficult. Then, many students will not study at home. Of course, some students maybe study what they want to learn, however, the problem is for those kids who can't study by themselves. Imagine, elementary school students, they don't know what study is important and how to do that. Then, some instructions such as homework is very important. Some of you may think homework is worthless, but giving homework meaning giving the opportunity to study is much more meaningful than do nothing or doing addictive games. That's why free time by abolishing homework is rather harmful to students.",
  "Pattern": {
    "PM": [
      [
        "X",
        "is negative"
      ],
      "support",
      [
        [
          "no X",
          "promotes",
          "Y"
        ],
        [
          "Y",
          "is good"
        ]
      ]
    ],
    "LO": [
      [
        "X",
        "is not negative"
      ],
      "support",
      [
        [
          [
            "no X",
            "promotes",
            "Y"
          ],
          [
            "Y",
            "is bad"
          ]
        ],
        [
          "given rationale/condition",
          "A"
        ]
      ]
    ],
    "Attack": [
      [
        [
          [
            [
              "no X",
              "promotes",
              "Y"
            ],
            [
              "Y",
              "is bad"
            ]
          ],
          [
            "given rationale/condition",
            "A"
          ]
        ],
        "contradicts",
        [
          [
            "no X",
            "promotes",
            "Y"
          ],
          [
            "Y",
            "is good"
          ]
        ]
      ],
      "nullify",
      [
        "X",
        "is negative"
      ]
    ],
    "Text spans": {
      "X": "Homework",
      "Y": "free time",
      "A": "what students will do during free time is just playing games and chatting using SNS in most cases or just sleeping"
    }
  },
  "Character offset of text spans": {
    "X": [
      34,
      42
    ],
    "Y": [
      206,
      215
    ],
    "A": [
      82,
      196
    ]
  }
}
{
  "PM": "Hello everyone. Today's topic is \"Homework should be abolished\". We have two points: The first point is \"free time\" and the second point is \"decrease burden on teachers\". I will explain the first point of \"free time\". We believe that if homework were to be abolished, we could have more free time. As a result, we could do more of what we really wanted like club activities, hobbies, or playing with friends. In my case, I go to tennis club after class until 5:00 pm and then I go to cram school until 8:00 pm. After this full day, I arrive at my home around 8:40 pm to eat dinner and take a shower. At nearly 10:00 pm I start my homework. I have a lot of homework. As a result, I go to bed late at night at nearly 1:00 am in the morning and I don't have the opportunity to sleep for a long period of time. It is not healthy. Therefore, homework should be abolished. Thank you.",
  "LO": "They said that students will have more free time by abolishing homework. However, what students will do during free time is just playing games and chatting using SNS in most cases or just sleeping as they said. It is because human is lazy in nature. Doing hard thing is usually difficult. Then, many students will not study at home. Of course, some students maybe study what they want to learn, however, the problem is for those kids who can't study by themselves. Imagine, elementary school students, they don't know what study is important and how to do that. Then, some instructions such as homework is very important. Some of you may think homework is worthless, but giving homework meaning giving the opportunity to study is much more meaningful than do nothing or doing addictive games. That's why free time by abolishing homework is rather harmful to students.",
  "Pattern": {
    "PM": [
      [
        "X",
        "is negative"
      ],
      "support",
      [
        [
          "no X",
          "promotes",
          "Y"
        ],
        [
          "Y",
          "is good"
        ]
      ]
    ],
    "LO": [
      [
        "X",
        "is not negative"
      ],
      "support",
      [
        [
          [
            "no X",
            "promotes",
            "Y"
          ],
          [
            "Y",
            "is bad"
          ]
        ],
        [
          "given rationale/condition",
          "A"
        ]
      ]
    ],
    "Attack": [
      [
        [
          [
            [
              "no X",
              "promotes",
              "Y"
            ],
            [
              "Y",
              "is bad"
            ]
          ],
          [
            "given rationale/condition",
            "A"
          ]
        ],
        "contradicts",
        [
          [
            "no X",
            "promotes",
            "Y"
          ],
          [
            "Y",
            "is good"
          ]
        ]
      ],
      "nullify",
      [
        "X",
        "is negative"
      ]
    ],
    "Text spans": {
      "X": "Homework",
      "Y": "free time",
      "A": "what students will do during free time is just playing games and chatting using SNS in most cases or just sleeping"
    }
  },
  "Character offset of text spans": {
    "X": [
      34,
      42
    ],
    "Y": [
      206,
      215
    ],
    "A": [
      82,
      196
    ]
  }
```

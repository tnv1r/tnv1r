
```python
#!/usr/bin/python
# -*- coding: utf-8 -*-


class FrontendEngineer:
    def __init__(self):
        self.name = "Taseen Tanvir"
        self.location = "27.2046° N, 77.4977° E"
        self.role = "Frontend Engineer"
        self.blog = "https://tanvir.io/"
        self.surfaceweb_portfolio="https://tanvir.io/"
        self.darkweb_portfolio="http://aq5at63kdmryyjicrbuuda6rqqlbmdj2qjysprkotimvgmeklyl6u2qd.onion"
        self.mastered = {
            "frontend": ["React", "Redux", "Next.js", "Vue.js", "HTML", "CSS", "JavaScript", "Chakra UI", "Tailwindcss"],
            "backend": ["NodeJS"],
            "database": ["MongoDB", "Firestore"],
            "tools": ["GIT", "Github", "Gitlab", "Vscode"],
            "misc": ["GNU/Linux"]
        }
        self.knowledge_base = [
            "Software Enginnering",
            "Machine Learning",
            "Deep Learning",
            "Computer Vision",
        ]
        self.knowledge_base.insert(0, "Backend Engineering")

    def say_hi(self):
        print(
            """
            Hello my friend, thanks for dropping by! This is {name}, I live in {location}. 
            I work as a {role} and recently I am focusing on {focus} for my personal growth. 
            Till now I've experience in working with {frontend}, keeping {backend} as backend.
            Even though I've less experience working with databases specially SQL, 
            I somehow managed to master some NoSQL databases like: {database}.
            Over the time, I got familiarized with so many tools including: {tools}.
            Other miscellaneous collection of tools that I got under my belt involves {misc}.
            I also have a wide range of interests, but some of them are {knowledge_base}. 
            In my free time, I write down tips and lecture notes on my personal tech blog, which can be found here: {blog}.
            If you wanna know more about me, take a look at my portfolio here: {surfaceweb_portfolio}, 
            or if you are a dark web person then visit here: {darkweb_portfolio}.
            """.format(
                name=self.name,
                location=self.location,
                role=self.role,
                frontend=", ".join(mastered["frontend"])
                backend=", ".join(mastered["backend"])
                database=", ".join(mastered["database"])
                tools=", ".join(mastered["tools"])
                misc=", ".join(mastered["misc"])
                focus=self.knowledge_base[0],
                knowledge_base=", ".join(self.knowledge_base[1:]),
                blog=self.blog,
                surfaceweb_portfolio=self.surfaceweb_portfolio,
                darkweb_portfolio=self.darkweb_portfolio
            )
        )


me = FrontendEngineer()
me.say_hi()

```

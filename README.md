
```python
#!/usr/bin/python
# -*- coding: utf-8 -*-


class FrontendEngineer:
    def __init__(self):
        self.name = "Taseen Tanvir"
        self.location = "27.2046° N, 77.4977° E"
        self.role = "Frontend Engineer"
        self.blog = "https://tanvir.io/"
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
            Even though I've less experience working with databases specially SQL, I managed to master databases like: {database}.
            Over the time, I also got familiarized with so many tools including: {tools}.
            Other miscellaneous collection of tools I got under my belt inclues: {misc}.
            I have wide interests, but most of them are {knowledge_base}. 
            I write down tips and lecture notes on my personal tech blog, which can be found here: {blog}
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
            )
        )


me = FrontendEngineer()
me.say_hi()

```

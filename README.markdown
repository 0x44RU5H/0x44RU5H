```python
#!/usr/bin/python3

from human import Human
from human.utilities import shelter, food, water, computer, internet, novels

class AarushGupta:
    def __init__(self):
        self.name = "Aarush Gupta"
        self.website = "https://theaarushgupta.com"
        self.email = "aarush@theaarushgupta.com"
        self.discord = "0x44RU5H#2101"
        self.pronouns = "He/Him"
        self.rolesInSociety = ["Student", "Programmer", "Writer"]
        self.knows = ["Python", "HTML", "CSS", "Javascript", "NodeJS", "SQL", "Bash"]
        self.workingOn = {
            "Website" : self.website,
            "AshMail" : (
                "https://ashmail.theaarushgupta.com",
                "https://github.com/ashmail",
                "https://github.com/ashmail/ashmail"
            )
        }

    def run(self, shelter, food, water, computer, internet, novels):
        human = Human([attribute for attribute in dir(self) if "__" not in attribute])
        human.startLife(shelter, food, water, computer, internet, novels)
        return human.happy

if __name__ == "__main__":
    aarushgupta = AarushGupta()
    happy = aarush.run(shelter, food, water, computer, internet, novels)
    print(happy)
```

```
$ vim aarushgupta.py
$ chmod +x aarushgupta.py
$ python3 ./aarushgupta.py
True
```

# Yaktocat (Octocat's alter-ego)

![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png "Yaktocat")

### What is a cat?

*The typical cat on GitHub is an Octocat. However, Yaktocat is also here!*

```Typescript
interface Cat {
  name: string;
  color: string;
}

class Octocat implements Cat {
  name: string;
  color: string;
  numberOfArms: number;

  constructor(name: string, color: string, numberOfArms: number) {
    this.name = name;
    this.color = color;
    this.numberOfArms = numberOfArms;
  }
}

class Yaktocat implements Cat {
  name: string;
  color: string;
  hasCrown: boolean;

  constructor(name: string, color: string, hasCrown: boolean) {
    this.name = name;
    this.color = color;
    this.hasCrown = hasCrown;
  }
}
```

#### How can I instantiate a cat?

You can instantiate an Octocat or Yaktocat by using the `new` keyword:

```Typescript
const octo = new Octocat("Octocat", "black", 8);
const yakto = new Yaktocat("Yaktocat", "blue", true);

console.log("Octocat: ", octo);
console.log("Yaktocat: ", yakto);
```

The output of this should look like this:

```bash
[LOG]: "Octocat: ",  Octocat: {
  "name": "Octocat",
  "color": "black",
  "numberOfArms": 8
} 
[LOG]: "Yaktocat: ",  Yaktocat: {
  "name": "Yaktocat",
  "color": "blue",
  "hasCrown": true
} 
```

#### Steps to instantiating and testing a cat

- [x] instantiate the cat
- [x] test the output by printing
- [ ] run a test that checks if the cat is null/undefined
- [ ] run a test that checks the name, color, and numberOfArms/hasCrown

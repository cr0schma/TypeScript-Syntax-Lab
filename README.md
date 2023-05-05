### C#
```csharp
public class Dog
{
	public string Name { get; set; }
	public string Breed { get; set; }

	public Dog(string name, string breed)
	{
    	Name = name;
    	Breed = breed;
	}

	public string Bark()
	{
    	return "Woof!";
	}
}

string[] dogBreeds = new string[] { "Labrador", "Golden Retriever", "Bulldog" };

public string GetRandomBreed(string[] breeds)
{
	Random random = new Random();
	int index = random.Next(breeds.Length);
	return breeds[index];
}
```
### JavaScript
```javascript
class Dog
{
	constructor(Name, Breed)
	{
    	this.Name = Name;
    	this.Breed = Breed;
	}

	Bark()
	{
    	return "Woof!";
	}
}

// Instantiate class and run Bark method
const dog = new Dog("Tahoe", "Pomski");
console.log(dog.Bark());

let dogBreeds = ["Labrador", "Golden Retriever", "Bulldog"];
console.log(dogBreeds);

function GetRandomBreed(breeds)
{
	let index = Math.floor(Math.random() * breeds.length) + 1;
	return breeds[index];
}
console.log(GetRandomBreed(dogBreeds))
```
### Typescript
```typescript
class Dog
{
	Name: string;
	Breed: string;

	constructor(Name: string, Breed: string)
	{
    	this.Name = Name;
    	this.Breed = Breed;
	}

	Bark(): string
	{
    	return "Woof!";
	}
}

// Instantiate class and run Bark method
const dog: Dog = new Dog("Tahoe", "Pomski");
console.log(dog.Bark());

let dogBreeds: string[] = ["Labrador", "Golden Retriever", "Bulldog"];
console.log(dogBreeds);

function GetRandomBreed(breeds: string[]): string
{
	let index: number = Math.floor(Math.random() * breeds.length) + 1;
	return breeds[index];
}
console.log(GetRandomBreed(dogBreeds))
```

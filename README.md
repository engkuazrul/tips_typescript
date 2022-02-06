# Typescript Tips and Tricks

###### Children
- JSX.Element
- JSX.Element | JSX.Element[];
- React.ReactNode;
- React.ReactChildren;
- React.ReactChild[];

###### CSS Properties
- React.CSSProperties


###### Set State Without a Default Value
```
  const [character, setCharacter] = React.useState<CharacterType | null>(null);
```

###### Change Event
```
changeCount = (event: ChangeEvent<HTMLInputElement>) => {
    this.setState({count: +event.target.value});
  }
```

###### Submit Event
```
const handleSubmit = (event: React.FormEvent<HTMLFormElement>) => {
  event.preventDefault();
  onSubmit(value);
};
```

###### Combination/Extends of Type
```
type PizzaData = {
  numberOfPeople: number;
  slicesPerPerson: number;
  slicesPerPie: number;
};

type PizzaState = PizzaData & { pizzasNeeded: number };

/*
numberOfPeople: number;
slicesPerPerson: number;
slicesPerPie: number;
pizzasNeeded: number 
*/
```

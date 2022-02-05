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

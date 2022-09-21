## Build Tower

```
export const towerBuilder = (nFloors: number): string[] => {
  let tower = [];
  let end:number = nFloors;
  let space:number = end-1;
  for(let i = 0;i<nFloors;i++){
    tower.push(' '.repeat(space)+ '*'.repeat(1 + (i*2)) + ' '.repeat(space))
    space -=1;
  }
  return tower
}
```

## Meeting

```
export function meeting(s: string): string {
  return s.toUpperCase()
          .split(';')
          .map(n => '(' + n.split(':').reverse().join(', ') +')')
          .sort() 
          .join('');
}
```

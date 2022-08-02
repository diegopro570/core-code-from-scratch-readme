## Who likes it?

To give a brief introduction about how this works, it will take names on the argument of the function and will return wether who likes it or not.
```
let likes = names => {
    let factor = names.length
        if(factor==0){
            return "no one likes this"
        }
        else if(factor==1){
            return names[0]+" likes this"
        }
        else if(factor == 2){
            return names[0]+" and "+ names[1]+" like this"
        }
        else if(factor == 3){
            return names[0]+", "+names[1]+" and "+ names[2]+" like this"
        }
        else{
            return names[0]+", "+names[1]+" and "+(factor-2)+" others like this"
        }
    
}
```


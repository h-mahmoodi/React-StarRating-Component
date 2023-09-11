# React-StarRating-Component
 React Star Rating Component |  A simply reusable , flexible and standalone react component

 # How To Use Component
 
Available props :

max : (number) (default=5) Set total rate count

color : (string) (default="#d4851a") Set star rating color

size : (number) (default=30) Set shape and font size in px

className : (string) (default="") Set custom class attr for add more user's style

message : (array) (default=[]) Set custom message for each rate

onSetRating : (function) (default=()) Set a function to return rating value


Example of usage :

First Add component file (StarRating.jsx) to src/component
Then use it every where(import it before use)

Code Example :

 Define a useState to recieve rating output number to use anywhere:
 const [rating, setRating] = useState(null);
 
  
    <div className="App">
    
        <StarRating
          max={5}
          size={35}
          color="blue"
          className="hesam"
          onSetRating={setRating}
          message={["very bad", "bad", "medium", "good", "very good"]}
        />
        
        <p>Rate is {rating}</p>
        
    </div>



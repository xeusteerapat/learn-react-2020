# Props

Props is stand for properties, props in react is a system for passing data from a parent component to a child component (or a nested component). Then we can make it easy to reusable.

OK, let's see the example. Suppose we have a component nested like this.

*note: I have used a library called `faker.js` for dummy data also semantic-ui for ui*

```javascript
// index.js
import React from 'react';
import ReactDOM from 'react-dom';
import CommentDetail from './CommentDetail.js';

const App = () => {
  return (
    <div className="ui container comments">
      <CommentDetail />
    </div>
  );
};

ReactDOM.render(<App />, document.getElementById('root'));
```

and `CommentDetail.js`

```javascript
import React from 'react';
import faker from 'faker';

const CommentDetail = () => {
  return (
    <div>
      <div className="comment">
        <a href="/" className="avatar">
          <img src={faker.image.avatar()} alt="avatar" />
        </a>
        <div className="content">
          <a href="/" className="author">
            Sam
          </a>
          <div className="metadata">
            <span className="date">Today 5:00PM</span>
          </div>
          <div className="text">Wowww! That's great!</div>
        </div>
      </div>
      <div className="comment">
        <a href="/" className="avatar">
          <img src={faker.image.avatar()} alt="avatar" />
        </a>
        <div className="content">
          <a href="/" className="author">
            Sam
          </a>
          <div className="metadata">
            <span className="date">Today 5:00PM</span>
          </div>
          <div className="text">Wowww! That's great!</div>
        </div>
      </div>
      <div className="comment">
        <a href="/" className="avatar">
          <img src={faker.image.avatar()} alt="avatar" />
        </a>
        <div className="content">
          <a href="/" className="author">
            Sam
          </a>
          <div className="metadata">
            <span className="date">Today 5:00PM</span>
          </div>
          <div className="text">Wowww! That's great!</div>
        </div>
      </div>
    </div>
  );
};

export default CommentDetail;
```

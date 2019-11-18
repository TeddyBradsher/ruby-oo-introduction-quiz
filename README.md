## Quiz: Ruby Object Orientation Fundamentals

???

# Ruby Object Orientation Fundamentals

?: A class is like a blueprint that defines how to build an object.

(X) True ( ) False

?: To define a class, what syntax is used?

( )
```ruby
Class Pet
end
```
( )
```ruby
Class pet
end
```
( )
```ruby
class pet
end
```
(X)
```ruby
class Pet
end
```

?: 

```ruby
class Pet
  def initialize(name)
    @name = name
  end
end

dog = Pet.new("Harpo")
```

In the example above, `Pet.new("Harpo")` will instantiate a new instance of the `Pet` class.

(X) True ( ) False

?: 

```ruby
class Pet
  def initialize(name)
    @name = name
  end

  def name=(name)
    @name = name
  end

  def name
    @name
  end
end

dog = Pet.new
```

`Pet.new` in this example will instantiate a new instance of the `Pet` class?
( ) True (X) False

?: 

```ruby
class Pet
  def initialize(name)
    @name = name
  end

  def name=(name)
    @name = name
  end

  def name
    @name
  end
end
```

```ruby
rabbit = Pet.new("Jabby")
rabbit.name
```

`rabbit.name` in this example will output `Jabby`.
(X) True ( ) False

?: 

```ruby
class Pet
  def initialize(name)
    @name = name
  end

  def name
    @name
  end
end
```

```ruby
rabbit = Pet.new("Jabby")
rabbit.name("Chokola")
```

What will `rabbit.name("Chokola")` in this example return?
( ) Chokola ( ) Jabby (X) ArgumentError ( ) None of the Above

?:

```ruby
class Pet
  def initialize(name)
    @name = name
  end

  def name=(name)
    @name = name
  end
  
  def name
    @name
  end
end
```

```ruby
rabbit = Pet.new("Jabby")
rabbit.name = "Chokola
```

In the example above, What will `rabbit.name = "Chokola"` return?
(X) Chokola ( ) Jabby ( ) ArgumentError ( ) None of the Above

?: A macro in Ruby is code that returns more Ruby code.

(X) True ( ) False

?: The `attr_reader` macro, followed by the attribute name, creates a setter method.

( ) True (X) False

?:

```ruby
class Pet

  attr_reader :name
  attr_writer :name

end
```

```ruby
buddy = Pet.new("Buddy")
buddy.name = "Chappie"
```

Considering the code above, what will `buddy.name` output?

( ) Buddy (X) Chappie ( ) ArgumentError ( ) None of the Above

?:

```ruby
class Pet

  attr_accessor :name

end
```

```ruby
buddy = Pet.new("Buddy")
```

What will `buddy.name` in this example output?

(X) Buddy ( ) Chappie ( ) ArgumentError ( ) None of the Above

???

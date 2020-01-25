---
layout: post
title:      "Setting up has many through in models"
date:       2020-01-25 04:54:32 +0000
permalink:  setting_up_has_many_through_in_models
---


In my Rails project, it was important to make sure associations was set in properly. Setting up the "has many through" associations is simple. The example on [this site](https://guides.rubyonrails.org/association_basics.html) is pretty good I think. From the link it looks like this:
```
class Physician < ApplicationRecord
  has_many :appointments
  has_many :patients, through: :appointments
end
 
class Appointment < ApplicationRecord
  belongs_to :physician
  belongs_to :patient
end
 
class Patient < ApplicationRecord
  has_many :appointments
  has_many :physicians, through: :appointments
end
```

Appointment belongs to both patient and physician. Both patient and physician can have many appointments, and through appointments they have many physicians or patients. There are more than 3 models in my Rails project, but connecting different models is still pretty much the same. User, Recipe, RecipeIngredient, and Ingredient are just some of the models used, but we'll focus on Recipe, RecipeIngredient, and Ingredient for this.
```
class Recipe < ApplicationRecord
   has_many :recipe_ingredients
   has_many :ingredients, through: :recipe_ingredients
end

class RecipeIngredient < ApplicationRecord
   belongs_to :ingredient
   belongs_to :recipe
end

class Ingredient < ApplicationRecord
   has_many :recipe_ingredients
   has_many :recipes, through: :recipe_ingredients
end

```

RecipeIngredient belongs to recipe and ingredient. Both recipe and ingredieny can have many recipe_ingredients, and through recipe_ingredients they have many recipes or ingredients.

The pattern to remember is that the model that joins two other models will usually have "belongs_to" at least twice (one for each of the other two models).



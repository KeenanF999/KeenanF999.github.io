---
layout: post
title: Latest from Developer Course
---

I call this week "Going deeper down the rabbit hole" this one example helped me to understand the through: command in Rails.  Or more of the relation data together in different relationships (1:M or M:M)

class Group < ActiveRecord::Base
has_many   :users
has_many   :avatars, through: :users
end

class User < ActiveRecord::Base
belongs_to :group
has_one    :avatar
end

class Avatar < ActiveRecord::Base
belongs_to :user
end

class Animals < ActiveRecords::Base
belongs_to :zpp
End

Also keeping the naming associations not the same as instance method. 

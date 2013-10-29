To Do:

User login and user authentication with Devise
User profiles (user#show) and user view and a way to update profiles
Add avatar photos to profiles with paperclip

Discussion boards:

	with subcategories, like subreddits
	category has_many: :posts
	post has_many: comments
	comment belongs_to :post

	Category name:string description:text
	Post title:string body:text link:string author/user_id up_votes:integer down_votes:integer
	Comment title:string body:text author/user_id up_votes:integer down_votes:integer

Private messages:

from:user_id
to:user_id
title:string
body:text

messages#new
messages#read (all messages where to: == current_user.id)


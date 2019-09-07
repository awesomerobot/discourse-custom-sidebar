# discourse-custom-sidebar

This theme component adds a sidebar populated by a post. Intended to be used along with the [Atlas theme](https://github.com/awesomerobot/atlas), but with some styling it can be utilized with other themes.

1. First you need to create a topic containing the desired sidebar’s content. This topic must be publicly accessible, but you can make it unlisted so it doesn’t show up in topic lists.

2. Once the topic is created, you then need to find the ID of the post. If you right click the post’s content, and then select “Inspect” you’ll see the page’s source. Within this you can search (control or command + F) for the text `data-post-id` which is followed by the post ID.

3. You can then add a new sidebar to a category by visiting the discourse-custom-sidebar theme component (admin > customize > themes) and entering the value in the input under “Theme Settings” formatted as “category,post,ID” — so for example to add a sidebar to the Staff category: `Staff,post,3`

4. To add a sidebar to the generic /latest, /top, /unread, /new topic lists, you can use all as the category name. So for example `all,post,3`

# Sách Lược - Blog

Chào mừng bạn đến với blog của tôi! 📚

## Bài viết gần đây

{% for post in site.posts %}
- [{{ post.title }}]({{ site.baseurl }}{{ post.url }}) - {{ post.date | date: "%d/%m/%Y" }}
{% endfor %}

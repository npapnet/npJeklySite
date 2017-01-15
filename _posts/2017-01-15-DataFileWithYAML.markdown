---
layout: post
title:  "Χρήση YAML για αυτόματη παρουσίαση δεδομένων"
date:   2017-01-15 22:51:10 +0200
categories: jekyll update
---


# Εισαγωγή

Στο παρόν ποστ παρουσιάζεται η χρήση αρχείων δεδομένων για την αυτόματη δημιουργία posts.

## Χρήση

[Χρήση αρχείων δεδομένων](http://jekyllrb.com/docs/datafiles/)


<p><b>Feedback</b></p>
<p>{{site.data.books.feedback}}</p>

<p><b>Block</b></p>
<p>{{site.data.books.block}}</p>

# Παράδειγμα με συντήρηση

Το συγκεκριμένο παράδειγμα χρησιμοποιεί το αρχείο **_data/books.yml** μέσα στο φάκελο δεδομένων.

<ul>
{% for item in site.data.books.bikes %}
<li>{{item.title}}</li>
{% endfor %}
</ul>

# Περαιτέρω πληροφορίες

Για περισσότερες πληροφορίες δείτε [Jekyll docs][jekyll-datafiles]. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh].

[YAML Tutorial](http://idratherbewriting.com/documentation-theme-jekyll/mydoc_yaml_tutorial)


[jekyll-datafiles]: http://jekyllrb.com/docs/datafiles/
[jekyll-gh]:   https://github.com/jekyll/jekyll

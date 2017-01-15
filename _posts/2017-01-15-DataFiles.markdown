---
layout: post
title:  "Χρήση αρχείων δεδομένων για την παραγωγή posts"
date:   2017-01-15 20:52:10 +0200
categories: jekyll update
---

# Εισαγωγή

Στο παρόν ποστ παρουσιάζεται η χρήση αρχείων δεδομένων για την αυτόματη δημιουργία posts.

## Χρήση

[Χρήση αρχείων δεδομένων](http://jekyllrb.com/docs/datafiles/)

# Παράδειγμα

Το συγκεκριμένο παράδειγμα χρησιμοποιεί το αρχείο **_data/members.csv** μέσα στο φάκελο δεδομένων.

<ul>
{% for member in site.data.members %}
  <li>
    <a href="https://github.com/{{ member.github }}">
      {{ member.name }}
    </a>
  </li>
{% endfor %}
</ul>

# Παράδειγμα με συντήρηση

Το συγκεκριμένο παράδειγμα χρησιμοποιεί το αρχείο **_data/maintenance.csv** μέσα στο φάκελο δεδομένων.

<ul>
{% for member in site.data.maintenance %}
  <li>
    {{ member.Date }}     {{ member.Function }}
  </li>
{% endfor %}
</ul>

# Περαιτέρω πληροφορίες

Για περισσότερες πληροφορίες δείτε [Jekyll docs][jekyll-datafiles]. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh].



[jekyll-datafiles]: http://jekyllrb.com/docs/datafiles/
[jekyll-gh]:   https://github.com/jekyll/jekyll

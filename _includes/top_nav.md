<link rel="stylesheet" href="{{site_base_url}}assets/css/styles.css">


![OWASP NBTX Chapter Logo](assets/images/nbtx_logo.png)
<br/>
<br/>


<nav class="ch-top-nav">
<ul>
{% if include.page == "home" %}
<li><a href=""><strong>Home Page</strong></a></li>
{%else%}
<li><a href="/">Home Page</a></li>
{%endif%}
{%if include.page == "pastactivities"%}
<li><a href=""><strong>Past Activities</strong></a></li>
{%else%}
<li><a href="pastactivities">Past Activities</a></li>
{%endif%}
{%if include.page == "sponsorship"%}
<li><a href=""><strong>Sponsor Us!</strong></a></li>
{%else%}
<li><a href="sponsorship">Sponsor Us!</a></li>
{%endif%}
</ul>
</nav>
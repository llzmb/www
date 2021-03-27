:template: {{year}}/generic.html

Schedule
========

Write the Docs is more than a conference.
Each year we organize a wide range of events so that people can come together, collaborate, and learn from each other in different ways.

.. contents::
    :local:
    :depth: 1
    :backlinks: none


{% if flaghashike or flaghasboat %}

{{date.day_one.dotw}}, {{date.day_one.date}}
--------------------------------------------------

{% endif %}

{% if flaghashike %}

Hike
~~~~

The only event scheduled on Saturday is the :doc:`annual hike to Pittock Mansion </conf/{{shortcode}}/{{year}}/outing>`.
If you get into town early, join us on the hike and take the chance to explore Portland in all of its glory.

* **Where**: Lower Macleay Park or Macleay Park Entrance.
* **When**: **{{ date.day_two.hike_time }} {{ tz }}**
* **Details**: :doc:`Annual hike to Pittock Mansion </conf/{{shortcode}}/{{year}}/outing>`

{% endif %}

{% if flaghasboat %}

Boat Ride
~~~~~~~~~

The only event scheduled on Saturday is the :doc:`Prague Boat Ride </conf/{{shortcode}}/{{year}}/outing>`.
If you get into town early, join us and experience Prague from the water.

Further details will be announced later.

{% endif %}


{{date.day_two.dotw}}, {{date.day_two.date}}
-----------------------------------------

The Writing Day and Welcome Reception will be held in our **{{about.venue}}**.

{% if flaghasfood %}

*Breakfast and lunch will be provided, as well as snacks and drinks all day.*

{% endif %}

Writing Day
~~~~~~~~~~~

* **Where**: {{about.venue}}
* **When**: **{{ date.day_two.writing_day_time }} {{ tz }}**
* **Details**: :doc:`Writing Day documentation sprints </conf/{{shortcode}}/{{year}}/writing-day>`

.. separator to fix list formatting

{% if flaghasschedule %}

{% with day_schedule=schedule.writing_day %}
{% include "include/schedule2021.rst" %}
{% endwith %}

{% else %}
  A detailed schedule will be announced soon.
{% endif %}

{% if flaghasfood %}

Reception
~~~~~~~~~

We encourage everyone to drop by on Sunday evening for the conference reception.
We're hoping to have some fun activities planned for the evening online.

* **Where**: {{about.venue}}, {{about.mainroom}}
* **When**: **17:00-20:00 {{ tz }}**

{% endif %}


.. raw:: html

   <hr>


{{date.day_three.dotw}}, {{date.day_three.date}}
-----------------------------------------

{{ date.day_three.summary }}

{% if flaghasfood %}

*Breakfast and lunch will be provided, as well as snacks and drinks all day.*

{% endif %}

Conference Talks
~~~~~~~~~~~~~~~~

* **Where**: {{about.venue}}
* **When**: **10:00-18:00 {{ tz }}**
* **Details**: :doc:`/conf/{{shortcode}}/{{year}}/speakers`

.. separator to fix list formatting

{% if flaghasschedule %}

{% with day_schedule=schedule.talks_day1 %}
{% include "include/schedule2021.rst" %}
{% endwith %}

{% else %}
    A detailed schedule will be announced soon.
{% endif %}

Unconference
~~~~~~~~~~~~

The unconference sessions run in parallel to the main conference talks.

* **Where**: {{about.venue}}, {{about.unconfroom}}
* **When**: **{{ date.day_three.unconference_time }} {{ tz }}**
* **Details**: :doc:`/conf/{{shortcode}}/{{year}}/unconference`

Social Event
~~~~~~~~~~~~

The official Write the Docs social!
Further details will be announced later,
but expect some music and games,
and bring your favorite beverage to your computer :)


.. raw:: html

   <hr>


{{date.day_four.dotw}}, {{date.day_four.date}}
-----------------------------------------

{{ date.day_four.summary }}

{% if flaghasfood %}

*Breakfast and lunch will be provided, as well as snacks and drinks all day.*

{% endif %}

Conference Talks
~~~~~~~~~~~~~~~~

* **Where**: {{about.venue}}
* **When**: **{{ date.day_three.talk_time }} {{ tz }}**
* **Details**: :doc:`/conf/{{shortcode}}/{{year}}/speakers`

.. separator to fix list formatting

{% if flaghasschedule %}

{% with day_schedule=schedule.talks_day2 %}
{% include "include/schedule2021.rst" %}
{% endwith %}

{% else %}
  A detailed schedule will be announced soon.
{% endif %}

{% if flaghasjobfair %}

Job Fair
~~~~~~~~

We'll be holding a job fair on Tuesday morning!

* **Where**: {{about.venue}}, {{about.unconfroom}}
* **When**: **{{ date.day_four.job_fair_time }} {{ tz }}**
* **Details**: :doc:`/conf/{{shortcode}}/{{year}}/job-fair`

{% endif %}

Unconference
~~~~~~~~~~~~

The unconference sessions run in parallel to the main conference talks.

* **Where**: {{about.venue}}, {{about.unconfroom}}
* **When**: **{{ date.day_four.unconference_time }} {{ tz }}**
* **Details**: :doc:`/conf/{{shortcode}}/{{year}}/unconference`

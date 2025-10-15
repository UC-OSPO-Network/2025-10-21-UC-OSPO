---
layout: workshop      # DON'T CHANGE THIS.
# More detailed instructions (including how to fill these variables for an
# online workshop) are available at
# https://carpentries.github.io/workshop-template/customization/index.html
venue: "UC OSPO Network"        # brief name of the institution that hosts the workshop without address (e.g., "Euphoric State University")
address: "online"      # full street address of workshop (e.g., "Room A, 123 Forth Street, Blimingen, Euphoria"), videoconferencing URL, or 'online'
country: "us"      # lowercase two-letter ISO country code such as "fr" (see https://en.wikipedia.org/wiki/ISO_3166-1#Current_codes) for the institution that hosts the workshop
language: "en"     # lowercase two-letter ISO language code such as "fr" (see https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for the workshop
latitude: "45"        # decimal latitude of workshop venue (use https://www.latlong.net/)
longitude: "-1"       # decimal longitude of the workshop venue (use https://www.latlong.net)
humandate: "Oct 21-22, 2025"    # human-readable dates for the workshop (e.g., "Feb 17-18, 2020")
humantime: "12:00 - 2:00 pm PDT"    # human-readable times for the workshop e.g., "9:00 am - 4:30 pm CEST (7:00 am - 2:30 pm UTC)"
startdate: 2025-10-21      # machine-readable start date for the workshop in YYYY-MM-DD format like 2015-01-01
enddate: 2025-10-22        # machine-readable end date for the workshop in YYYY-MM-DD format like 2015-01-02
instructor: ["Tim Dennis", "Reid Otsuji"] # boxed, comma-separated list of instructors' names as strings, like ["Laura Langdon", "Betty Jennings", "Betty Snyder"]
helper: ["Laura Langdon", "Karla Padilla", "Hannah Sutherland"]     # boxed, comma-separated list of helpers' names, like ["Marlyn Wescoff", "Fran Bilas", "Ruth Lichterman"]
email: ["datascience+ospo@ucla.edu"]    # boxed, comma-separated list of contact email addresses for the host, lead instructor, or whoever else is handling questions, like ["marlyn.wescoff@example.org", "fran.bilas@example.org", "ruth.lichterman@example.org"]
collaborative_notes: https://pad.carpentries.org/2025-uc-ospo  # optional: URL for the workshop collaborative notes, e.g. an Etherpad or Google Docs document (e.g., https://pad.carpentries.org/2015-01-01-euphoria)
eventbrite:           # optional: alphanumeric key for Eventbrite registration, e.g., "1234567890AB" (if Eventbrite is being used)
what3words:           # optional: what3words (https://what3words.com) address of the workshop venue, without leading slashes e.g. "globe.lessening.computers"
---

{% comment %} See instructions in the comments below for how to edit specific sections of this workshop template. {% endcomment %}

{% comment %}
HEADER

Edit the values in the block above to be appropriate for your workshop.
If the value is not 'true', 'false', 'null', or a number, please use
double quotation marks around the value, unless specified otherwise.
And run 'make workshop-check' *before* committing to make sure that changes are good.
{% endcomment %}

{% comment %}
Check DC curriculum
{% endcomment %}

{% if site.carpentry == "dc" %}
{% unless site.curriculum == "dc-astronomy" or site.curriculum == "dc-ecology" or site.curriculum == "dc-genomics" or site.curriculum == "dc-geospatial" or site.curriculum == "dc-image" or site.curriculum == "dc-socsci" %}
<div class="alert alert-warning">
It looks like you are setting up a website for a Data Carpentry curriculum but you haven't specified the curriculum type in the <code>_config.yml</code> file (current value in <code>_config.yml</code>: "<strong>{{ site.curriculum }}</strong>", possible values: <code>dc-image</code>, <code>dc-astronomy</code>, <code>dc-ecology</code>, <code>dc-genomics</code>, <code>dc-socsci</code>, or <code>dc-geospatial</code>). After editing this file, you need to run <code>make serve</code> again to see the changes reflected.
</div>
{% endunless %}
{% endif %}

{% comment %}
Check SWC curriculum
{% endcomment %}

{% if site.carpentry == "swc" %}
{% unless site.curriculum == "swc-inflammation" or site.curriculum == "swc-gapminder" %}
<div class="alert alert-warning">
It looks like you are setting up a website for a Software Carpentry curriculum but you haven't specified the curriculum type in the <code>_config.yml</code> file (current value in <code>_config.yml</code>: "<strong>{{ site.curriculum }}</strong>", possible values: <code>swc-inflammation</code>, or <code>swc-gapminder</code>). After editing this file, you need to run <code>make serve</code> again to see the changes reflected.
</div>
{% endunless %}
{% endif %}

<!-- REGISTRATION (Zoom) -->
<h2 id="registration">Registration</h2>
<div class="alert alert-info" role="region" aria-label="Registration links">
  <p><strong>Please register on Zoom for each session:</strong></p>
  <ul class="list-unstyled">
    <li>
      <strong>Session 1 — Getting Started with Better Research Software</strong><br>
      Tue, Oct 21 · 12:00–2:00 PM PDT<br>
      <a class="btn btn-primary btn-sm" href="https://ucla.zoom.us/meeting/register/ffG30PhZSVSSMPg-04y2dw#/registration" target="_blank" rel="noopener">
        Register for Session 1
      </a>
    </li>
    <li class="mt-3">
      <strong>Session 2 — Writing Clearer, Better-Structured Code</strong><br>
      Wed, Oct 22 · 12:00–2:00 PM PDT<br>
      <a class="btn btn-primary btn-sm" href="https://ucla.zoom.us/meeting/register/H8mm-16jTlek7Et7zaB3uA" target="_blank" rel="noopener">
        Register for Session 2
      </a>
    </li>
  </ul>

  <p class="mt-3 mb-0">
    <em>This workshop is designed for researchers, graduate students, and early-career Research Software Engineers (RSEs) 
    who already have some experience with Python, Git, and the shell.</em>
  </p>

  <hr>

  <p class="mb-0"><strong>Forthcoming Sessions (dates TBA):</strong></p>
  <ul>
    <li>Code Correctness: Writing and automating tests</li>
    <li>Software Documentation: Creating effective READMEs and metadata</li>
    <li>Open Software Management & Collaboration: GitHub issues, citation, multi-developer workflows</li>
    <li>Wrap-Up: FAIR principles and broader practices in research software</li>
  </ul>
</div>


<h2 id="general">General Information</h2>

{% comment %}
INTRODUCTION

Edit the general explanatory paragraph below if you want to change
the pitch.
{% endcomment %}

<p>
<strong><a href="https://carpentries.org">The Carpentries</a></strong> project comprises the <a
href="{{site.swc_site}}">Software Carpentry</a>, <a href="{{site.dc_site}}">Data Carpentry</a>, and
<a href="{{site.lc_site}}">Library Carpentry</a> communities of Instructors, Trainers, Maintainers,
helpers, and supporters who share a mission to teach foundational computational and data science
skills to researchers.
<p align="center">
  <em>
  <strong>Want to learn more and stay engaged with The Carpentries?</strong> Carpentries Clippings is The Carpentries' biweekly newsletter, where we share community news, community job postings, and more.
Sign up to receive future editions and read our full archive: <a href="https://carpentries.org/newsletter/">https://carpentries.org/newsletter/</a>
  </em>
</p>
{% if site.carpentry == "swc" %}
{% include swc/intro.html %}
{% elsif site.carpentry == "dc" %}
{% include dc/intro.html %}
{% elsif site.carpentry == "lc" %}
{% include lc/intro.html %}
{% endif %}

{% if site.pilot %}
This is a pilot workshop, testing out a lesson that is still under development. The lesson authors would appreciate any feedback you can give them about the lesson content and suggestions for how it could be further improved.
{% endif %}

{% comment %}
AUDIENCE

Explain who your audience is.  (In particular, tell readers if the
workshop is only open to people from a particular institution.
{% endcomment %}
{% if site.carpentry == "swc" %}
{% include swc/who.html %}
{% elsif site.carpentry == "dc" %}
{% include dc/who.html %}
{% elsif site.carpentry == "lc" %}
{% include lc/who.html %}
{% endif %}

{% comment %}
LOCATION

This block displays the address and links to maps showing directions
if the latitude and longitude of the workshop have been set.  You
can use https://www.latlong.net/ to find the lat/long of an
address.
{% endcomment %}
{% assign begin_address = page.address | slice: 0, 4 | downcase  %}
{% if page.address == "online" %}
{% assign online = "true_private" %}
{% elsif begin_address contains "http" %}
{% assign online = "true_public" %}
{% else %}
{% assign online = "false" %}
{% endif %}
{% if page.latitude and page.longitude and online == "false" %}
<p id="where">
  <strong>Where:</strong>
  {{page.address}}.
  Get directions with
  <a href="//www.openstreetmap.org/?mlat={{page.latitude}}&mlon={{page.longitude}}&zoom=16">OpenStreetMap</a>
  or
  <a href="//maps.google.com/maps?q={{page.latitude}},{{page.longitude}}">Google Maps</a>.
  {% if page.what3words %}
    What3Words location:
    <a href="https://what3words.com/{{page.what3words}}">///{{page.what3words}}</a>.
  {%endif %}
</p>
{% elsif online == "true_public" %}
<p id="where">
  <strong>Where:</strong>
  online at <a href="{{page.address}}">{{page.address}}</a>.
  If you need a password or other information to access the training,
  the instructor will pass it on to you before the workshop.
</p>
{% elsif online == "true_private" %}
<p id="where">
  <strong>Where:</strong> This training will take place online.
  The instructors will provide you with the information you will need to connect to this meeting.
</p>
{% endif %}

{% comment %}
DATE

This block displays the date and links to Google Calendar.
{% endcomment %}
{% if page.humandate %}
<p id="when">
  <strong>When:</strong>
  {{page.humandate}}; {{page.humantime}}
  {% include workshop_calendar.html %}
</p>
{% endif %}

{% comment %}
SPECIAL REQUIREMENTS

Modify the block below if there are any special requirements.
{% endcomment %}
<p id="requirements">
  <strong>Requirements:</strong>
  {% if online == "false" %}
    Participants must bring a laptop with a
    Mac, Linux, or Windows operating system (not a tablet, Chromebook, etc.) that they have administrative privileges on.
  {% else %}
    Participants must have access to a computer with a
    Mac, Linux, or Windows operating system (not a tablet, Chromebook, etc.) that they have administrative privileges on.
  {% endif %}
  They should have a few specific software packages installed (listed <a href="#setup">below</a>).
</p>

{% comment %}
ACCESSIBILITY

Modify the block below if there are any barriers to accessibility or
special instructions.
{% endcomment %}
<p id="accessibility">
  <strong>Accessibility:</strong>
  We are committed to making this workshop
  accessible to everybody. 
{% if online == "false" %}
  The workshop organizers have checked that:
<p>
  <ul>
    <li>The room is wheelchair / scooter accessible.</li>
    <li>Accessible restrooms are available.</li>
  </ul>
{% endif %}
</p>
<p>We are dedicated to providing a positive and accessible learning environment for all. 
  We do not require participants to provide documentation of disabilities or disclose any unnecessary personal information. 
  However, we do want to help create an inclusive, accessible experience for all participants. 
  We encourage you to share any information that would be helpful to make your Carpentries experience accessible.
  To request an accommodation for this workshop, please fill out the 
  <a href="https://carpentries.typeform.com/to/B2OSYaD0">accommodation request form</a>.
  If you have questions or need assistance with the accommodation form please <a href="mailto:team@carpentries.org">email us</a>.
</p>
<p>
  <a href="https://glosario.carpentries.org/">Glosario</a> is a multilingual glossary 
  for computing and data science terms. The glossary helps 
  learners attend workshops and use our lessons to make sense of computational and programming jargon written in English by offering it 
  in their native language. Translating data science terms also provides a teaching tool for Carpentries Instructors to reduce barriers 
  for their learners.
</p>

{% comment %}
WORKSHOP RECORDINGS

Modify or remove the block below if you plan to record the workshop.
{% endcomment %}
<p id="recordings">
  <strong>Workshop Recordings:</strong>
  Carpentries workshops are designed to be interactive rather than lecture-based, with lessons that build upon one another.
  To foster a positive online learning environment, we strongly recommend that participants join in real time.
  As a result, workshop recordings are not recommended and may not be available to learners.
</p>
{% comment %}
CONTACT EMAIL ADDRESS

Display the contact email address set in the configuration file.
{% endcomment %}
<p id="contact">
  <strong>Contact:</strong>
  Please email
  {% if page.email %}
  {% for email in page.email %}
  {% if forloop.last and page.email.size > 1 %}
  or
  {% else %}
  {% unless forloop.first %}
  ,
  {% endunless %}
  {% endif %}
  <a href='mailto:{{email}}'>{{email}}</a>
  {% endfor %}
  {% else %}
  to-be-announced
  {% endif %}
  for more information.
</p>

<p id="roles">
  <strong>Roles:</strong>
  To learn more about the roles at the workshop (who will be doing what),
  refer to <a href="https://carpentries.org/workshop_faq/#what-are-the-roles-of-everyone-participating-in-a-workshop">our Workshop FAQ</a>.
</p>

{% comment %}
WHO CAN ATTEND?

If you would like to specify who can attend the workshop,
you can use the section below.

Move the 'endcomment' tag above the beginning of the following
<p> tag to make this section visible.

Edit the text to match who can attend the workshop. For instance:
- This workshop is open to affiliates to ABC university.
- This workshop is open to the public.
- If you are interested in attending this workshop, contact me@example.com
  for more information

<p id="who-can-attend">
    <strong>Who can attend?:</strong>
    This workshop is open to ....
</p>
{% endcomment %}

<hr/>

{% comment%}
CODE OF CONDUCT
{% endcomment %}
<h2 id="code-of-conduct">Code of Conduct</h2>

<p>
Everyone who participates in Carpentries activities is required to conform to the <a href="https://docs.carpentries.org/policies/coc/">Code of Conduct</a>. This document also outlines how to report an incident if needed.
</p>

<p class="text-center">
  <a href="https://goo.gl/forms/KoUfO53Za3apOuOK2">
    <button type="button" class="btn btn-info">Report a Code of Conduct Incident</button>
  </a>
</p>
<hr/>


{% comment %}
Collaborative Notes

If you want to use an Etherpad, go to

https://pad.carpentries.org/YYYY-MM-DD-site

where 'YYYY-MM-DD-site' is the identifier for your workshop,
e.g., '2015-06-10-esu'.

Note we also have a CodiMD (the open-source version of HackMD)
available at https://codimd.carpentries.org
{% endcomment %}
{% if page.collaborative_notes %}
<h2 id="collaborative_notes">Collaborative Notes</h2>

<p>
We will use this <a href="{{ page.collaborative_notes }}">collaborative document</a> for chatting, taking notes, and sharing URLs and bits of code.
</p>
<hr/>
{% endif %}


{% comment %}
SURVEYS - DO NOT EDIT SURVEY LINKS
{% endcomment %}
<h2 id="surveys">Surveys</h2>
<p>Please be sure to complete these surveys before and after the workshop.</p>
{% if site.carpentry == "incubator" %}
<p><a href="{{ site.incubator_pre_survey }}">Pre-workshop Survey</a></p>
<p><a href="{{ site.incubator_post_survey }}">Post-workshop Survey</a></p>
{% elsif site.incubator_pre_survey or site.incubator_post_survey %}
<div class="alert alert-danger">
WARNING: you have defined custom pre- and/or post-survey links for
a workshop not configured for The Carpentries Incubator
(the value of `curriculum` is not set to `incubator` in `_config.yml`).
Please comment out the `incubator_pre_survey` and `incubator_post_survey` fields
in `_config.yml` or, if this workshop is teaching a lesson in the Incubator,
change the value of `carpentry` to `incubator`.
</div>
{% else %}
<p><a href="{{ site.pre_survey }}{{ site.github.project_title }}">Pre-workshop Survey</a></p>
<p><a href="{{ site.post_survey }}{{ site.github.project_title }}">Post-workshop Survey</a></p>
{% endif %}

<hr/>


{% comment %}
SCHEDULE

Show the workshop's schedule.

Small changes to the schedule can be made by modifying the
`schedule.html` found in the `_includes` folder for your
workshop type (`swc`, `lc`, or `dc`). Edit the items and
times in the table to match your plans. You may also want to
change 'Day 1' and 'Day 2' to be actual dates or days of the
week.

For larger changes, a blank template for a 4-day workshop
(useful for online teaching for instance) can be found in
`_includes/custom-schedule.html`. Add the times, and what
you will be teaching to this file. You may also want to add
rows to the table if you wish to break down the schedule
further. To use this custom schedule here, replace the block
of code below the Schedule `<h2>` header below with
`{% include custom-schedule.html %}`.
{% endcomment %}

<h2 id="schedule">Schedule</h2>

{% if site.carpentry == "swc" %}
{% include swc/schedule.html %}
{% elsif site.carpentry == "dc" %}
{% include dc/schedule.html %}
{% elsif site.carpentry == "lc" %}
{% include lc/schedule.html %}
{% elsif site.carpentry == "incubator" %}
This workshop is teaching a lesson in 
<a href="https://carpentries-incubator.org/">The Carpentries Incubator</a>. Please check <a href="{{site.incubator_lesson_site}}">the lesson homepage</a> for a list of lesson sections and estimated timings.
{% endif %}

{% comment %}
Edit/replace the text above if you want to include a schedule table.
See the contents of the _includes/custom-schedule.html file for an example of
how one of these schedule tables is constructed.
{% endcomment %}

{% if site.pilot %}
The lesson taught in this workshop is being piloted and a precise schedule is yet to be established. The workshop will include regular breaks. Please <a href="mailto:{{page.email}}">contact the workshop organisers</a> if you would like more information about the planned schedule.
{% endif %}

<hr/>


{% comment %}
SETUP

Delete irrelevant sections from the setup instructions.  Each
section is inside a 'div' without any classes to make the beginning
and end easier to find.

This is the other place where people frequently make mistakes, so
please preview your site before committing, and make sure to run
'tools/check' as well.
{% endcomment %}

<h2 id="setup">Setup</h2>

<p>
  To participate in a
  {% if site.carpentry == "swc" %}
  Software Carpentry
  {% elsif site.carpentry == "dc" %}
  Data Carpentry
  {% elsif site.carpentry == "lc" %}
  Library Carpentry
  {% endif %}
  workshop,
  you will need access to software as described below.
  In addition, you will need an up-to-date web browser.
</p>
<p>
  We maintain a list of common issues that occur during installation as a reference for instructors
  that may be useful on the
  <a href = "{{site.swc_github}}/workshop-template/wiki/Configuration-Problems-and-Solutions">Configuration Problems and Solutions wiki page</a>.
</p>

{% comment %}
For online workshops, the section below provides:
- installation instructions for the Zoom client
- recommendations for setting up Learners' workspace so they can follow along
  the instructions and the videoconferencing

If you do not use Zoom for your online workshop, edit the file
`_includes/install_instructions/videoconferencing.html`
to include the relevant installation instructions.
{% endcomment %}
{% if online != "false" %}
{% include install_instructions/videoconferencing.html %}
{% endif %}

{% comment %}
These are the installation instructions for the tools used
during the workshop.
{% endcomment %}

{% if site.carpentry == "swc" %}
{% include swc/setup.html %}
{% elsif site.carpentry == "dc" %}
{% include dc/setup.html %}
{% elsif site.carpentry == "lc" %}
{% include lc/setup.html %}
{% elsif site.carpentry == "incubator" %}
Please check the "Setup" page of
<a href="{{site.incubator_lesson_site}}">the lesson homepage</a> for instructions to follow
to obtain the software and data you will need to follow the lesson.
<!-- HIGH-VIS SETUP CALLOUT -->
<div class="alert alert-warning" role="region" aria-label="Software setup">
  <h3 class="mb-3">🔧 Prepare Your Computer Before the Workshop</h3>
  <p><strong>Before you arrive (required): Complete the software setup for this lesson.</strong></p>
  <p class="mb-2">Follow the official instructions here:</p>
  <p>
    <a class="btn btn-primary btn-sm" href="https://carpentries-incubator.github.io/better-research-software/#software-setup" target="_blank" rel="noopener">Software Setup (overview)</a>
    <a class="btn btn-primary btn-sm" href="https://carpentries-incubator.github.io/better-research-software/installation-instructions.html" target="_blank" rel="noopener">Installation Instructions (step-by-step)</a>
  </p>

  <hr>

  <p class="mb-1"><strong>Quick pre-flight check (run these in your terminal):</strong></p>
  <ul class="mb-2">
    <li><code>git --version</code></li>
    <li><code>python --version</code> (Python 3.x)</li>
    <li><code>pip --version</code></li>
  </ul>

  <p class="mb-1"><strong>Tips:</strong></p>
  <ul class="mb-2">
    <li>Windows users: open <em>Command Prompt</em> or <em>PowerShell</em>. macOS/Linux: open <em>Terminal</em>.</li>
    <li>If any command fails, revisit the installation page and re-run the relevant step.</li>
  </ul>

  <p class="mb-0"><em>Need help?</em> Join 15 minutes early or email <a href="mailto:datascience+ospo@ucla.edu">datascience+ospo@ucla.edu</a>.</p>
</div>

{% endif %}

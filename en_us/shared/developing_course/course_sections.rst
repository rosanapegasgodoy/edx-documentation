.. _Developing Course Sections:

###################################
Developing Course Sections
###################################

To develop sections in your course, you must first understand the following
topics.

.. contents::
  :local:
  :depth: 2

****************************
What Is a Section?
****************************

A section is the topmost category in your course. A section can represent a
time period in your course, a chapter, or another organizing principle. A
section contains one or more subsections.

********************************
Viewing Sections in the Outline
********************************

The following example shows four sections, all collapsed, in the course
outline.

.. image:: ../../../shared/images/sections-outline.png
 :alt: Four sections in the outline.
 :width: 600

******************************
The Learner View of a Section
******************************

In the LMS, learners see section names in the course outline on the **Course**
page, with subsections listed under the section name. Learners click
subsection names to access the units in the selected
:ref:`subsection<Developing Course Subsections>`.

In the following example, two section names are indicated with a box outline.

.. image:: ../../../shared/images/sections_student.png
 :alt: The learner view of the course outline, with two section titles
       indicated with a box outline.

.. _Sections and Visibility to Learners:

************************************************
Sections and Visibility to Learners
************************************************

Learners cannot see any content in a section if the section's release date is
unscheduled or has not passed.

If a section's release date has passed, learners can see content in the section
if:

* The release date for the subsection that contains that content has passed.
* The unit has been published.
* The unit is not hidden from learners.

************************************************
Release Statuses of Sections
************************************************

As an course author, you control the release status of sections.  For the
content of a section to be visible to learners, the section must be released.
See the following topics for more information about the possible release
statuses of sections.

.. contents::
  :local:
  :depth: 1

========================
Unscheduled
========================

If you do not change the :ref:`course start date<Set Start and End Dates>`
default value, ``1/1/2030 00:00:00 UTC``, when you create a new section, its
release date will appear as ``Unscheduled``. When the section release date is
unscheduled, learners cannot see any content in that section, regardless of
the publishing status of that content.

If you have modified the course start date, when you create a new section, the
default release date is the course start date.

On the Studio **Course Outline** page, each unscheduled section appears with a
gray bar next to the section display name.

To make the content available to learners, you must schedule the release date.

==========
Scheduled
==========

A section that is scheduled for release on a future date will not be visible to
learners until after the release date. Regardless of the publishing status of
content within the section, the entire section will not visible to learners.

The following example shows how a section that is scheduled for release
displays in the outline, summarized with a green bar.

On the Studio **Course Outline** page, each scheduled section appears with a
green bar next to the section display name.

The scheduled date must pass for the section to be visible to learners.

===========================
Released
===========================

A section that is released is visible to learners; however, learners see only
subsections within the section that are also released, and units that are
published.

On the Studio **Course Outline** page, each released section appears with a
blue bar next to the section display name.

==================================
Released with Unpublished Changes
==================================

If you change a unit in a released section but do not publish the changes,
learners see the last published version of the modified unit.

On the Studio **Course Outline** page, each released section that has
unpublished changes appears with a yellow bar next to the section display name.
When you expand the section, the unit that has unpublished changes is visible.

You must publish the unit for learners to see the updates.

===========================
Staff Only Content
===========================

A section can contain a unit that is hidden from learners and available to
members of the course team only. That unit is not visible to learners,
regardless of the release date of the section or subsection.

On the Studio **Course Outline** page, each section that includes a unit with
staff only content appears with a black bar next to the section display name.

.. _Create a Section:

****************************
Create a Section
****************************

If you do not change the :ref:`course start date<Set Start and End Dates>`
default value, ``1/1/2030``, when you create a new section, its release date
will be ``Unscheduled``.

If you have modified the course start date, when you create a new section, the
default release date is the course start date.

.. caution::
 If the course start date is in the past, newly created sections are
 immediately visible to learners.

To create a new section, follow these steps.

#. On the **Course Outline** page, select **New Section**. This option appears
   at both the top of the page and below the current sections in the outline.

   A new section appears at the end of the course content, with the section
   name selected.

#. Enter the name for the new section. A descriptive name can help learners
   locate content in the course. It can also help you select content when
   you analyze performance in edX Insights.

#. :ref:`Add subsections<Create a Subsection>` to the new section as needed.

It is recommended that you :ref:`test course content <Testing Your Course
Content>` as you create new sections.

********************************
Change a Section Name
********************************

To edit a section name, move your cursor over the section name to show the
**Edit** icon.

.. image:: ../../../shared/images/section-edit-icon.png
  :alt: The Edit Section Name icon.
  :width: 500

Select the **Edit** icon next to the section name. The name field becomes
editable. Enter the new name, and then tab or click outside of the field to
save the name.

.. _Set a Section Release Date:

********************************
Set a Section Release Date
********************************

To set the section release date, follow these steps.

#. Select the **Configure** icon in the section box.

   .. image:: ../../../shared/images/section-settings-box.png
    :alt: The section settings icon circled.
    :width: 500

   The **Settings** dialog box opens.

#. Enter the release date and time for the section.

  .. note::
   The time that you set is in Coordinated Universal Time (UTC). You might want
   to verify that you have specified the time that you intend by using a time
   zone converter such as `Time and Date Time Zone Converter
   <http://www.timeanddate.com/worldclock/converter.html>`_.

#. Select **Save**.

For more information, see :ref:`Release Dates`.

.. _Set Section Highlights for Weekly Course Highlight Messages:

***********************************************************
Set Section Highlights for Weekly Highlight Emails
***********************************************************

.. only:: Partners

  To improve learner engagement, edX can send an automatic weekly email message
  to learners who enroll in self-paced courses. These weekly messages
  correspond to course sections in Studio, and contain three to five
  "highlights" for each upcoming course section. A highlight is a brief
  description of an important concept, idea, or activity. EdX provides most of
  the text for this weekly course highlight email in a template, and you enter
  the highlights for the email in Studio. For an example email, see
  :ref:`Weekly Course Highlight Message Text`.

  For more information about email messages that edX sends to learners
  automatically, see :ref:`Automatic Email`.

  When you add highlights for a section, keep the following information in
  mind.

  * Each highlight has a limit of 250 characters.
  * If you include a hyperlink in your highlights, we recommend that you use a
    URL shortener to shorten any long URLs, and then enter the shortened URL in
    the highlight. Most HTML email renderers automatically convert URLs into
    hyperlinks.
  * **If you do not add highlights for a section, edX does not send learners a
    message for that section.** We strongly encourage you to add highlights for
    all course sections.

    Additionally, edX uses consecutive numbers for each message, even if some
    sections do not have highlights. For example, if you add highlights for
    section 1 and section 3, but you do not add highlights for section 2,
    learners receive a message on day 14 that contains the highlights for
    section 3.

  * Learners who enroll in the course before you enter highlights do not
    receive any course highlight messages for the duration of the course. To
    make sure that all of your learners receive weekly course highlight
    messages, enter highlights for each section before any learners enroll in
    your course.
  * If you update a highlight for a section, the change takes effect
    immediately for all subsequent messages that contain that highlight.

.. only:: Open_edX

  If your Open edX system adminstrator has configured your instance of the Open
  edX platform to send course highlight emails, you can send automatic email
  messages to learners in your course that contain three to five "highlights"
  of upcoming course content. A highlight is a brief description of an
  important concept, idea, or activity in the section. Your Open edX system
  administrator provides the template for this course highlight email, and
  you enter the highlights for the email in Studio.

  For more information, contact your Open edX system administrator.

.. note::
   The highlights that you specify persist when you re-run your course.

.. only:: Partners

  .. _Weekly Course Highlight Message Text:

  ====================================
  Weekly Highlight Email Text
  ====================================

  The following example shows the edX email template with three example
  highlights.

  .. include:: ../../../shared/developing_course/course_highlight_message_text.rst

.. _Set Section Highlights:

=========================================
Send Weekly Highlight Emails
=========================================

To send weekly highlight emails to your learners, you must first set highlights
for each section. When you have set section highlights, you then enable the
**Weekly Highlight Emails** setting.

The number of highlights that you have set for a section is
visible in the course outline, below the name of the section.

.. image:: ../../../shared/images/NumSectionHighlights.png
 :alt: The Course Outline page, showing a section name and "3 Section
     Highlights" under the name.

.. _Set Course Section Highlights:

Set Course Section Highlights
**********************************

.. only:: Partners

   If you do not enter highlights for a section, the edX platform does not send
   an email message for that section. Instead, edX sends an email message for
   the next section that has highlights.

.. only:: Open_edX

  .. note::
    If your Open edX system adminstrator has not configured your instance of
    the Open edX platform to send weekly course highlight messages, learners do
    not receive messages even if you enable highlights and enter highlights for
    each section.

To set highlights for a course section, follow these steps.

#. On the **Course Outline** page, locate the section you want, and then select
   **Section Highlights** under the section name.
#. In the **Highlights for <section name>** dialog box, enter three to five
   highlights for the section. Enter one highlight in each field. Each
   highlight can include up to 250 characters.
#. Select **Save**.

.. only:: Partners

  .. note::
    You can also enter course highlights in OLX.

.. _Enable Weekly Course Highlight Messages:

Enable Weekly Highlight Emails
********************************************

.. only:: Partners

  .. note::
   If you do not enable highlights, the edX platform does not send weekly
   course highlight emails, even if you enter highlights for one or more
   sections.

After you have set and reviewed the highlights for each course section, and are
ready to start sending highlights for the course, you enable weekly highlight
emails.

To enable weekly highlight emails, follow these steps.

.. note::
  You cannot disable weekly highlight emails after you enable them. If you do
  not want to send weekly highlight emails after you enable them, you can
  delete highlights in all sections.

#. On the **Course Outline** page, locate the **Weekly Highlight
   Emails** setting, and then select **Enable Now**.
#. In the dialog box that opens, select **Enable**.

.. _Publish all Units in a Section:

********************************
Publish All Units in a Section
********************************

To publish all new and changed units in a section, select the **Publish** icon
in the box for the section.

.. image:: ../../../shared/images/outline-publish-icon-section.png
 :alt: Publishing icon for a section.
 :width: 500

.. note::
 The **Publish** icon only appears when there is new or changed content within
 the section.

For more information about statuses and visibility to learners, see :ref:`Unit
Publishing Status`.

.. _Hide a Section from Students:

********************************
Hide a Section from Learners
********************************

You can hide all content in a section from learners, regardless of the status
of subsections and units within the section.

For more information, see :ref:`Content Hidden from Students`.

To hide a section from learners, follow these steps.

#. Select the **Configure** icon in the section box.

   .. image:: ../../../shared/images/section-settings-box.png
    :alt: The section settings icon circled.
    :width: 500

   The **Settings** dialog box opens.

#. In the **Section Visibility** section, select **Hide from learners**.

#. Select **Save**.

Now, none of the content in the section is visible to learners.

To make the section visible to learners, repeat these steps and deselect **Hide
from learners**.

.. warning::  When you deselect **Hide from learners** for a section, not all
   content in the section is necessarily made visible to learners. If you
   explicitly set a subsection or unit to be hidden from learners, it remains
   hidden from learners. Unpublished units remain unpublished, and changes to
   published units remain unpublished.


********************************
Delete a Section
********************************

When you delete a section, you delete all subsections and units within the
section.

.. warning::
 You cannot restore course content after you delete it. To ensure you do not
 delete content you may need later, you can move any unused content to a
 section in your course that you set to never release.

To delete a section, follow these steps.

#. Select the **Delete** icon in the section that you want to delete.

  .. image:: ../../../shared/images/section-delete.png
   :alt: The section with Delete icon circled.
   :width: 500

2. When you receive the confirmation prompt, select **Yes, delete this
   section**.

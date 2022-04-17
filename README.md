# Software_engineering_project3
# Projec№3: activity monitoring
  The software house OnTimeSoftware develops software on contract,
usually at fixed time, fixed price, and with specified functionality and
quality. One of the hardest problems is to detect early on that an activity
will take longer than expected. If you can detect it early, it is possible to
help the developer currently carrying out the activity, for instance by letting
a seasoned expert review the work and offer guidance. If you detect the
problem late, the activity may have run off the track, be costly to correct,
and it will soon hamper many other activities.
  Seasoned project managers know that they can get an early warning in
this way: The developer responsible for a given activity records every day
how many hours he has worked on the activity, and every weekend he gives
an estimate of the remaining number of hours. Project management now
computes an estimate of the total number of hours for the activity:
  *total expected = hours spent + hours remaining*
In a straightforward activity this figure remains constant from week to
week, and when no hours remain, it is finished. If the figure starts
increasing, something is wrong, and help is most likely needed. Experience
is that the problem in this way can be detected between 60% and 80% into
the activity, while it otherwise tends to be detected when more than the total
expected time has been used.
  Unfortunately, the procedure is cumbersome to manage, and company
management wants to support it with an IT system. At the same time they
want a better record of the work hours per activity, which many developers
at present record many days too late. The recording is at present also used
for billing some of the customers, and for collecting experience data of
hours used for various sizes of projects.
  When staffing a project, department managers and project managers
have troubles getting an overview of who will be available in the period
where the project is carried out. They expect the system to give them an
overview of this too.
# Specification
  OnTimeSoftware has around 80 developers and around 40 open
projects with around 800 planned or running activities. Many projects run
for just a few months, but some run for a couple of years. Most developers
work on less than 10 activities at a time, but a few may work on more than
20 each week.
  Each project consists of a set of activities, usually planned weeks
before they start. An activity is primarily carried out by a single developer -
responsible for this activity - but sometimes other developers may assist for
some hours. OnTimeSoftware has experienced that project management is
much harder if more than one person is allocated to an activity. So they take
great care dividing projects into activities for a single person. There is also
a special 'overhead' project that consists of activities such as vacation,
illness, lunch and courses.
  Developers must on a daily basis record how much time they have
spent on their activities - with an accuracy of half an hour. The system must
remind them if they have forgotten. This recording is presently considered
annoying, and it is crucial that the system makes it easy. For instance it
must be easy to find the proper activity numbers.
  Developers must once a week (Friday or Monday) give an estimate of
the remaining time for all activities that they are responsible for. Again, the
system must remind them if they forget. When the responsible developer
reports that the remaining time is zero, the activity is finished and he doesn't
have to report remaining time any more.
  The project manager (or any other developer) must be able to create
projects and activities, and nominate a responsible developer for each
activity. To do this, he must be able to see when this developer will be
available. He must be able to see how the hours spent and the estimated
total develop over time. It is particularly important to identify activities that
have a growing estimated total or where little work is done. Finally, he must
be able to see who is responsible for this activity and what else this
developer is supposed to work on.
  Project managers and department managers will typically monitor
several projects in this way. It would be convenient if they can get a good
overview of the projects they watch particularly closely.
# Assumptions
  Employees use initials of up to four letters and people usually know
each other's initials. The company has already a system that records all
employees, invoices customers based on hours used, collects experience
data, plans projects with a Gantt diagram, etc. There is no reason to deal
with these issues in this project.
  Projects have a number and a name, e.g 9511DXP version B.
  An activity is denoted by the project number and an activity number.
Furthermore, it has a name, e.g.
  9511-12 Design of communication module.
  Your job is to develop alpha version of the proposed system for the
activity monitoring. This system should take into account the sides of the
developers and the project manager.
  Assume that the system runs on the web platform or mobile devices. 
Please add the model of authentication system before starting the dialogue
with users before they have been logged on. For the alpha testing you can
use the existing (or created) user data from database so that the system
should know who the user is.

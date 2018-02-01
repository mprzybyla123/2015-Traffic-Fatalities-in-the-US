# 2015-Traffic-Fatalities-in-the-US

{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {
    "slideshow": {
     "slide_type": "slide"
    }
   },
   "source": [
    "# MSDS 7331-401 Lab 1\n",
    "\n",
    "#### Project Team:\n",
    "+ Peter Byrd \n",
    "+ Matthew Przybyla  \n",
    "+ David Tran\n",
    "+ Amber Whelpley\n",
    "\n",
    "# National Highway Traffic Safety Administration - 2015 Traffic Accidents\n",
    "\n",
    "## Business Understanding\n",
    "\n",
    "A primary objective of the National Highway Traffic Safety Administration (NHTSA) is to reduce the staggering human toll and property damage caused by motor vehicle traffic crashes.  Each year, thousands of lives are lost, hundreds of thousands are injured, and billions of dollars are lost in property damage.  Understanding the factors related to automotive crashes is needed to design and implement programs that effectively reduce the impact on human lives and reduce the billions lost in damages.\n",
    "\n",
    "In 1975, the Fatality Analysis Reporting System (FARS) began collecting information about fatal crashes involving all types of vehicles.  The FARS system is used to identify highway safety problem areas, and provide a basis for regulatory and consumer information initiatives.\n",
    "\n",
    "FARS is directed by the National Center for Statistics and Analysis which is a component of NHTSA.  Trained state employees, called \"FARS Analysts,\" are responsible for gathering, translating, and transmitting their States' data to NCSA.  FARS data are obtained from varius States' documents, such as:\n",
    "+ Police Accident Reports\n",
    "+ Death Certificates\n",
    "+ State Vehicle Registration Files\n",
    "+ Coroner/Medical Examiner Reports\n",
    "+ State Drive Licensing Files\n",
    "+ State Highway Department Data\n",
    "+ Emergency Medical Services Reports\n",
    "+ Vital Statistics and other State Records\n",
    "\n",
    "All qualifying fatalities that occur within the 50 US states, District of Columbia, and Puerto Rico are recorded.  A qualifying case involves a motor vehicle traveling on a trafficway open to the public, and must have resulted in a death of a motorist or non-motorist within 30 days of the accident.\n",
    "\n",
    "A desired outcome from analysis of the FARS data is to determine the primary causes associated with traffic fatalities and to drive awareness for prevention programs.  Identification of strong correlation between traffic fatalities and other recorded attributes such as weather, dates, or intoxication can lead to successful prevention measures.  \n",
    "\n",
    "For the analysis performed here, we will focus on the *accident.csv* file found at https://www.kaggle.com/nhtsa/2015-traffic-fatalities. An effective model will determine the factors that lead to a higher death rate in fatal crashes. Our intention is to eventually use this data to assist in predicting whether an accident will have multiple fatalities using the information we have. We consider a successful outcome to be successful prediction approximately 80% of the time. Whether this goal is possible remains to be seen.\n",
    "\n",
    "A successful prediction algorithm could be used to guide prevention programs toward awareness of certain factors that lead to a higher impact on human life.\n",
    "\n",
    "## Data Understanding\n",
    "\n",
    "The *accident.csv* dataset consists of all qualifying fatal automotive accidents from 2015.  There are 52 fields of relevant accident information and the dataset contains 32,166 records.\n",
    "\n",
    "To start, let's import and explore the dataset for a better understanding of the scale and meaning for each attribute."
   ]
  },

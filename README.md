# Hot-Spot-Analysis-Project

Purpose

In this project, you will perform numerous spatial queries on a huge database that contains
geographic information and the real-time locations of the customers of a well-known taxi company.

Project Description

You will be utilizing Scala and Apache Spark in this project to create a solution that can extract crucial
data from the provided dataset, which can then be used to make operational and strategic choices.
The technology gives the client access to statistically significant geographic locations, which it can
utilize to plan its operations in advance and improve customer service.

Directions

Before getting started, download the following project files from the course
1. CSE 511_Hot Spot Analysis Project_Required Templates.zip
2. CSE 511_Hot Spot Analysis Project_yellow_trip_sample_100000.zip

In this project, you are required to do spatial hot spot analysis. In particular, you need to complete two
different hot spot analysis tasks.

Tasks

1. Hot Zone Analysis

This task will need to perform a range join operation on a rectangle datasets and a point dataset. For
each rectangle, the number of points located within the rectangle will be obtained. The hotter
rectangle means that it includes more points. So this task is to calculate the hotness of all the
rectangles.

2. Hot Cell Analysis

This task will focus on applying spatial statistics to spatio-temporal big data in order to identify
statistically significant spatial hot spots using Apache Spark. The topic of this task is from ACM
SIGSPATIAL GISCUP 2016.

The Problem Definition page is here: http://sigspatial2016.sigspatial.org/giscup2016/problem

The Submit Format page is here: http://sigspatial2016.sigspatial.org/giscup2016/submit

Special requirement (different from GIS CUP)

As stated in the Problem Definition page, in this task, you are asked to implement a Spark program to
calculate the Getis-Ord statistic of NYC Taxi Trip datasets. We call it "hot cell analysis"

To reduce the computation power need, we made the following changes:

1. The input will be "yellow_trip_sample_100000.csv" dataset.
   
2. Each cell unit size is 0.01 * 0.01 in terms of latitude and longitude degrees.

3. You only need to consider Pick-up Location.

4. We don't use Jaccard similarity to check your answer. However, you don't need to worry about
how to decide the cell coordinates because the code template generates cell coordinates. You
just need to write the rest of the task.

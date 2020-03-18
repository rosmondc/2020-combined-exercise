# Fone Dynamics Full Stack Development Coding Challenge

## Introduction

Thank you for your interest in working with us at Fone Dynamics!
We all love working with talented co-workers. This challenge is intended to help us evaluate where you are in your programming career so we can determine how you might fit within our company.

## The Challenge

### Background

In order to assess your ability to develop backend and frontend applications, we ask that you develop a RESTful API in C# .Net Core, with an accompanying Angular Frontend.

This exercise is intended for those who wish to complete both the Backend and Full Stack exercises.

### Setup

1. You must first fork this repo. If you do not have a GitHub account, you will need to first sign up in order to fork it.
2. Clone your forked repo and develop the application according to the requirements below.
3. Once you think you have completed the exercise to a satisfactory level, ensure all of your code has been committed to your forked repo and issue a Pull Request back to the FoneDynamics repo.

### Requirements

You have been tasked to build a HTTP RESTful API using C# .Net Core, with an Angular frontend.

#### Backend

You will need to set up a database of your choice, containing two tables:
- users; containing usernames and passwords
- customers; containing customer data such as id, name, number of employees, tags

The API will connect to the database and serve data. You will need to generate a token to be returned by the Authorization endpoint.

This API will incorporate two endpoints:

1. Authorization endpoint
2. Customer record endpoint - to be secured by the token generated by the authorization endpoint.

These endpoints do not require data to be inserted or updated, a simple retrieval of data from the database and presented via the API is fine.

The url/path of these endpoints is at your discretion.

The customer record endpoint should also provide a filter on the querystring to filter by at least 1 tag, and/or the following for number of employees:
- 1-10
- 11-50
- &gt;50

Please include the data in your database in your git repository with a plaintext database dump.

#### Frontend

Develop an AngularJS application which has two parts:
1. A login screen which authorizes via the authorization endpoint in the backend
2. Once authenticated, shows a table of customers with the data retrieved from the backend's customer endpoint

The customer table should provide filters on the following:
- tags
- number of employees - 1-10 employees, 11-50 employees, 50+ employees

Each column in the customer table should be able to be reordered by clicking on the appropriate heading (ascending/descending)

The customer table must not be viewable unless the user is authenticated.

## Questions?

If you have any questions around the implementation of this exercise, please open an Issue on the parent repository at https://github.com/fonedynamics

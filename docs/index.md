---
layout: page
---

# Who's Working API Documentation

Turn your app into a staffing solution

Who's Working is a cloud service that helps your shift managers find trained part-time workers and fill staffing positions. It's an ideal tool for quick service operations that experience last-minute staff changes. The lightweight API provides access to a list of trained part-time workers who might be available on short notice for a restaurant shift. The Who's Working API uses REST and returns HTTP response codes and responses encoded in JSON.

There are two resources.

**Workers** - Part-time workers who sign up for the Who's Working service. The Workers resource includes endpoints to create, retrieve, update, and delete user information.

**Shifts** - Available shifts in the restaurant created by the shift manager. Each shift describes the location, day and time, shift length, and warnings. The Shifts resource includes endpoints to create, retrieve, update, and delete shift records.

## Authentification

The Who's Working app uses [Basic Authentication](api/basic_auth.md).

## Quickstart

[Quickstart](api/quickstart_working.md)

## Tutorials

Learn how to do common tasks within the Who's Working service. Do this tutorial to set up your development system. Complete the set up once per development system.

* [Before you start a tutorial](tutorials/before-you-start-a-tutorial.md)

After your system is ready, open the tutorial and learn how to perform common tasks.

#### Shifts

* [Update a shift](tutorials/update-a-shift.md)
* Create a shift
* Edit a shift
* Delete a shift
* Get a shift by a property

#### Workers

* Create a new worker
* Update a specific worker's information
* Delete a worker
* Get a worker by a property

## API reference docs

Click a link to read detailed descriptions of the service's resources. The API reference docs refer to a `{server_url}` when they refer to the URL of a resource. The `{server_url}` value depends on the installation of the service. When running a local test, the `{server_url}` is generally `http://localhost:3000`.

* [Shifts resources](api/shifts-resources.md)
* [Workers resources](api/workers-resources.md)

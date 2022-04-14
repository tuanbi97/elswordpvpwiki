---
title: "Roles And Permissions"
linkTitle: "Roles And Permissions"
weight: 1
description: >
  Overview about Roles And Permissions in Palexy platform.
---

## Overview
In general, Palexy system allow companies to manage users by roles and permissions on store objects. An user needs an appropriate roles and store permission to be able to view/edit data of stores. 

## Roles
Currently we are supporting four kind of roles:
- **Company Business Analyst**: this role is mostly assigned to accounts that only need READ access to view store analytical data. They can be CEOs, CMOs, ...
- **Store Manager**: this roles is mostly assigned to accounts that need to update some store data like staffing data. They can be Store Manager, District Manager, Regional Manager, ...
- **Layout Editor**: this roles is mostly assigned to accounts that need to update store layouts. They can be Store Manager or Visual Merchandiser.
- **Admin**: this role is the higest authority and have all available permissions. Currently we only allow to have one Admin account for a company.

When create new account, you need to specify at least one of the above role for an account. 

## Store Permissions
Currently we only support granting permissions for store objects. There are three permission types:
- READ: Can access any data related to the store but cannot modify it
- READ & WRITE: Have READ permissionCan modify some information of the store depending on the role
- ADMIN: Have WRITE permission. Can share the store for other users

## Grant Store Permission to an Account
To understand how role and store permission work together. Let walk through some examples:
- We want our company accountant to be able to view store data but cannot modify it. In this case, we will create for him/her an account with role **Company Business Analyst**. Then we will grant permission to READ on all stores for that account. With **Company Business Analyst** role and READ permission, the account can only view store analytical data.
- We want our Visual Merchandiser to draw sections on store but do not want them to view store analytical data. In this case, we will create for him/her an account with role **Layout Editor** and grant permission to WRITE to all stores that he/she needs to update layout, since this account has only **Layout Editor** role, even if with WRITE permission, he/she cannot view store anlaytical data.
- We want our Visual Merchandiser to draw sections on store and also want them to be able to view store analytical data. In this case, we will create for him/her an account with 2 role **Layout Editor** and  **Company Business Analyst** and grant permission to WRITE to all stores that he/she needs to update layout.

For detail how to grant store permissions to an account, please refer to [Grant Store Permissions]({{< ref "_grant_permissions.md" >}})

## Permissions and Roles Tables
Below are summary of currently supported permissions for each roles:

<img src="https://storage.googleapis.com/palexy-static-files/documents/permissions_and_roles.jpg"
     alt="Permissions and Roles"/>


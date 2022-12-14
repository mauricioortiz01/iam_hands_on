# IAM Hands On

During this Hands On you will lean how to:
1. Create an IAM Group
1. Create an IAM user included in the IAM Group.
1. Create an IAM role, attach it to an IAM user and switch role to the user
1. Create a policy, attach it to an IAM user and test it.

## Deliverables


## IAM User Group Creation
1. Sign in to AWS Management Console and open the IAM Console
    <img src="img/sign_in_iam.png" width="600">
1. On the right navigation pane, choose User groups and then click Create group.
    <img src="img/choose_create_group.png" width="600">
1. For User group name, type the name of the group `Training`, don't do anything else, and click `Create Group`
1. You should now see the `Training` group

    <img src="img/created_training_group.png" width="600"> 

## IAM User Creation
1. In the navigation pane, choose Users and then choose Add Users.
    <img src="img/add_users.png" width="600">
1. Create user
    1. Type your name as the username
    1. Select `Password - AWS Management Console Access`
    1. Select `Custom Password`
    1. Enter a custom password
    1. **Uncheck** `Require password reset`

        <img src="img/create_user.png" width="600">
1. Click `Next: Permissions`
    1. Add User to the Training group

        <img src="img/add_user_to_training.png" width="600">
1. Click `Next: Tags`
1. Click `Next: Review`
1. Click `Create User`
1. Click  `Close`

# Create an IAM Role with Admin Access
1. Go to the IAM console, in the Navigation pane, choose Roles
1. Click `Create Role`

    <img src="img/create_role.png" width="600">
1. Configure Role
    1. Select AWS Account
    1. Select `This account` (*Copy the account number you will need it later*)
    1. Click Next

         <img src="img/configure_role.png" width="600">
    1. Search for `AdminstratorAccess` policy, select it, and click `Next`

        <img src="img/select_adminstrator_access.png" width="600">
    1. Name the role `AdminstratorAccess` and click `Create Role`

        <img src="img/name_role.png" width="600">
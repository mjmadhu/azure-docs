---
title: 'Tutorial: Azure AD SSO integration with RightAnswers'
description: Learn how to configure single sign-on between Azure Active Directory and RightAnswers.
services: active-directory
author: jeevansd
manager: CelesteDG
ms.reviewer: celested
ms.service: active-directory
ms.subservice: saas-app-tutorial
ms.workload: identity
ms.topic: tutorial
ms.date: 06/29/2022
ms.author: jeedes
---
# Tutorial: Azure AD SSO integration with RightAnswers

In this tutorial, you'll learn how to integrate RightAnswers with Azure Active Directory (Azure AD). When you integrate RightAnswers with Azure AD, you can:

* Control in Azure AD who has access to RightAnswers.
* Enable your users to be automatically signed-in to RightAnswers with their Azure AD accounts.
* Manage your accounts in one central location - the Azure portal.

## Prerequisites

To configure Azure AD integration with RightAnswers, you need the following items:

* An Azure AD subscription. If you don't have an Azure AD environment, you can get a [free account](https://azure.microsoft.com/free/).
* RightAnswers single sign-on enabled subscription.
* Along with Cloud Application Administrator, Application Administrator can also add or manage applications in Azure AD.
For more information, see [Azure built-in roles](../roles/permissions-reference.md).

## Scenario description

In this tutorial, you configure and test Azure AD single sign-on in a test environment.

* RightAnswers supports **SP** initiated SSO.

## Add RightAnswers from the gallery

To configure the integration of RightAnswers into Azure AD, you need to add RightAnswers from the gallery to your list of managed SaaS apps.

1. Sign in to the Azure portal using either a work or school account, or a personal Microsoft account.
1. On the left navigation pane, select the **Azure Active Directory** service.
1. Navigate to **Enterprise Applications** and then select **All Applications**.
1. To add new application, select **New application**.
1. In the **Add from the gallery** section, type **RightAnswers** in the search box.
1. Select **RightAnswers** from results panel and then add the app. Wait a few seconds while the app is added to your tenant.

## Configure and test Azure AD SSO for RightAnswers

Configure and test Azure AD SSO with RightAnswers using a test user called **B.Simon**. For SSO to work, you need to establish a link relationship between an Azure AD user and the related user in RightAnswers.

To configure and test Azure AD SSO with RightAnswers, perform the following steps:

1. **[Configure Azure AD SSO](#configure-azure-ad-sso)** - to enable your users to use this feature.
    1. **[Create an Azure AD test user](#create-an-azure-ad-test-user)** - to test Azure AD single sign-on with B.Simon.
    1. **[Assign the Azure AD test user](#assign-the-azure-ad-test-user)** - to enable B.Simon to use Azure AD single sign-on.
1. **[Configure RightAnswers SSO](#configure-rightanswers-sso)** - to configure the single sign-on settings on application side.
    1. **[Create RightAnswers test user](#create-rightanswers-test-user)** - to have a counterpart of B.Simon in RightAnswers that is linked to the Azure AD representation of user.
1. **[Test SSO](#test-sso)** - to verify whether the configuration works.

## Configure Azure AD SSO

Follow these steps to enable Azure AD SSO in the Azure portal.

1. In the Azure portal, on the **RightAnswers** application integration page, find the **Manage** section and select **single sign-on**.
1. On the **Select a single sign-on method** page, select **SAML**.
1. On the **Set up single sign-on with SAML** page, click the pencil icon for **Basic SAML Configuration** to edit the settings.

    ![Screenshot shows to edit Basic S A M L Configuration.](common/edit-urls.png "Basic Configuration")

4. On the **Basic SAML Configuration** section, perform the following steps:

    a. In the **Identifier (Entity ID)** text box, type a URL using the following pattern:
    `https://<subdomain>.rightanswers.com:<identifier>/portal`

    b. In the **Sign on URL** text box, type a URL using the following pattern:
    `https://<subdomain>.rightanswers.com/portal/ss/`

    > [!NOTE]
    > These values are not real. Update these values with the actual Identifier and Sign on URL. Contact [RightAnswers Client support team](https://uplandsoftware.com/rightanswers/contact/) to get these values. You can also refer to the patterns shown in the **Basic SAML Configuration** section in the Azure portal.

1. On the **Set up Single Sign-On with SAML** page, in the **SAML Signing Certificate** section, click **Download** to download the **Federation Metadata XML** from the given options as per your requirement and save it on your computer.

    ![Screenshot shows the Certificate download link.](common/metadataxml.png "Certificate")

1. On the **Set up RightAnswers** section, copy the appropriate URL(s) as per your requirement.

    ![Screenshot shows to copy configuration appropriate U R L.](common/copy-configuration-urls.png "Metadata")  

### Create an Azure AD test user

In this section, you'll create a test user in the Azure portal called B.Simon.

1. From the left pane in the Azure portal, select **Azure Active Directory**, select **Users**, and then select **All users**.
1. Select **New user** at the top of the screen.
1. In the **User** properties, follow these steps:
   1. In the **Name** field, enter `B.Simon`.  
   1. In the **User name** field, enter the username@companydomain.extension. For example, `B.Simon@contoso.com`.
   1. Select the **Show password** check box, and then write down the value that's displayed in the **Password** box.
   1. Click **Create**.

### Assign the Azure AD test user

In this section, you'll enable B.Simon to use Azure single sign-on by granting access to RightAnswers.

1. In the Azure portal, select **Enterprise Applications**, and then select **All applications**.
1. In the applications list, select **RightAnswers**.
1. In the app's overview page, find the **Manage** section and select **Users and groups**.
1. Select **Add user**, then select **Users and groups** in the **Add Assignment** dialog.
1. In the **Users and groups** dialog, select **B.Simon** from the Users list, then click the **Select** button at the bottom of the screen.
1. If you are expecting a role to be assigned to the users, you can select it from the **Select a role** dropdown. If no role has been set up for this app, you see "Default Access" role selected.
1. In the **Add Assignment** dialog, click the **Assign** button.

## Configure RightAnswers SSO

To configure single sign-on on **RightAnswers** side, you need to send the downloaded **Federation Metadata XML** and appropriate copied URLs from Azure portal to [RightAnswers support team](https://uplandsoftware.com/rightanswers/contact/). They set this setting to have the SAML SSO connection set properly on both sides.

> [!NOTE]
> Your RightAnswers support team has to do the actual SSO configuration. You will get a notification when SSO has been enabled for your subscription.

### Create RightAnswers test user

To enable Azure AD users to sign in to RightAnswers, they must be provisioned into RightAnswers. When RightAnswers, provisioning is an automated task so there is no action item for you.

Users are automatically created if necessary during the first single sign-on attempt.

> [!NOTE]
> You can use any other RightAnswers user account creation tools or APIs provided by RightAnswers to provision Azure AD user accounts.

## Test SSO

In this section, you test your Azure AD single sign-on configuration with following options. 

* Click on **Test this application** in Azure portal. This will redirect to RightAnswers Sign-on URL where you can initiate the login flow. 

* Go to RightAnswers Sign-on URL directly and initiate the login flow from there.

* You can use Microsoft My Apps. When you click the RightAnswers tile in the My Apps, this will redirect to RightAnswers Sign-on URL. For more information about the My Apps, see [Introduction to the My Apps](../user-help/my-apps-portal-end-user-access.md).

## Next steps

Once you configure RightAnswers you can enforce session control, which protects exfiltration and infiltration of your organization’s sensitive data in real time. Session control extends from Conditional Access. [Learn how to enforce session control with Microsoft Cloud App Security](/cloud-app-security/proxy-deployment-aad).
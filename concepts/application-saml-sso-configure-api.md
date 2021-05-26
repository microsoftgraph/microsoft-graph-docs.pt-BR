---
title: Use as APIs do Microsoft Graph para configurar o logon único baseado em SAML
description: Aprenda a economizar tempo usando as APIs do Microsoft Graph para automatizar a configuração de logon único baseado em SAML.
author: kenwith
localization_priority: Priority
ms.custom: scenarios:getting-started
ms.prod: applications
ms.openlocfilehash: 85d8d97897facb8be40fb5260de7f143a626f07e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665054"
---
# <a name="configure-saml-based-single-sign-on-for-your-application-using-the-microsoft-graph-api"></a><span data-ttu-id="6e66f-103">Configure o logon único baseado em SAML para seu aplicativo usando a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6e66f-103">Configure SAML-based single sign-on for your application using the Microsoft Graph API</span></span>

<span data-ttu-id="6e66f-104">Neste artigo, você aprenderá como criar e configurar um SSO (logon único) baseado em SAML para seu aplicativo no Azure AD (Azure Active Directory) usando a API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6e66f-104">In this article, you'll learn how to create and configure a SAML-based single sign-on (SSO) for your application in Azure Active Directory (Azure AD) using the Microsoft Graph API.</span></span> <span data-ttu-id="6e66f-105">A configuração do aplicativo inclui URLs básicas de SAML, uma política de mapeamento de declarações e o uso de um certificado para adicionar uma chave de assinatura personalizada.</span><span class="sxs-lookup"><span data-stu-id="6e66f-105">The application configuration includes basic SAML URLs, a claims mapping policy, and using a certificate to add a custom signing key.</span></span> <span data-ttu-id="6e66f-106">Após o aplicativo ser criado, atribua a ele um usuário como administrador.</span><span class="sxs-lookup"><span data-stu-id="6e66f-106">After the application is created, you assign a user to it to be an administrator.</span></span> <span data-ttu-id="6e66f-107">Em seguida, você pode usar uma URL para obter metadados SAML do Azure AD para configuração adicional do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6e66f-107">You then can use a URL to obtain Azure AD SAML metadata for additional configuration of the application.</span></span> 

<span data-ttu-id="6e66f-108">Este artigo usa um modelo de aplicativo Azure AD da AWS como exemplo, mas você pode usar as etapas deste artigo para qualquer aplicativo baseado em SAML na Galeria do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6e66f-108">This article uses an AWS Azure AD application template as an example, but you can use the steps in this article for any SAML-based app in the Azure AD Gallery.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e66f-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e66f-109">Prerequisites</span></span>

<span data-ttu-id="6e66f-110">Este tutorial assume que você está usando o Microsoft Graph Explorer, mas você pode usar o Postman ou criar seu próprio aplicativo cliente para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6e66f-110">This tutorial assumes that you are using Microsoft Graph Explorer, but you can use Postman, or create your own client app to call Microsoft Graph.</span></span> <span data-ttu-id="6e66f-111">Para chamar as APIs do Microsoft Graph neste tutorial, você precisa usar uma conta com a função de administrador global e as permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="6e66f-111">To call the Microsoft Graph APIs in this tutorial, you need to use an account with the global administrator role and the appropriate permissions.</span></span> <span data-ttu-id="6e66f-112">Para este tutorial, as permissões delegadas `Application.ReadWrite.All`,`AppRoleAssignment.ReadWrite.All`,`Policy.Read.All`,`Policy.ReadWrite.ApplicationConfiguration` e `User.ReadWrite.All` são necessárias.</span><span class="sxs-lookup"><span data-stu-id="6e66f-112">For this tutorial, the `Application.ReadWrite.All`, `AppRoleAssignment.ReadWrite.All`, `Policy.Read.All`, `Policy.ReadWrite.ApplicationConfiguration`, and `User.ReadWrite.All` delegated permissions are needed.</span></span> <span data-ttu-id="6e66f-113">Conclua as seguintes etapas para definir as permissões no Microsoft Graph Explorer:</span><span class="sxs-lookup"><span data-stu-id="6e66f-113">Complete the following steps to set permissions in Microsoft Graph Explorer:</span></span>

1. <span data-ttu-id="6e66f-114">Vá para o [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="6e66f-114">Go to [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
2. <span data-ttu-id="6e66f-115">Selecione **Entrar com a conta da Microsoft** e entre usando uma conta de administrador global do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6e66f-115">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator account.</span></span> <span data-ttu-id="6e66f-116">Uma vez acessado, você verá os detalhes da conta do usuário no painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="6e66f-116">After you successfully sign in, you can see the user account details in the left-hand pane.</span></span>
3. <span data-ttu-id="6e66f-117">Selecione o ícone de configurações à direita dos detalhes da conta do usuário e, em seguida, selecione **Selecionar permissões**.</span><span class="sxs-lookup"><span data-stu-id="6e66f-117">Select the settings icon to the right of the user account details, and then select **Select permissions**.</span></span>

    ![Selecionar as permissões do Microsoft Graph](./images/application-saml-sso-configure-api/set-permissions.png)
        
4. <span data-ttu-id="6e66f-119">Na lista de permissões, role e expanda **AppRoleAssignment (1)** e selecione a permissão **AppRoleAssignment.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="6e66f-119">In the list of permissions, scroll to and expand **AppRoleAssignment (1)**, and then select the **AppRoleAssignment.ReadWrite.All** permission.</span></span> <span data-ttu-id="6e66f-120">Role mais para baixo e expanda **Aplicativo (2)** e selecione a permissão **Application.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="6e66f-120">Scroll further down and expand **Application (2)**, and then select the **Application.ReadWrite.All** permission.</span></span> <span data-ttu-id="6e66f-121">Continue e expanda **Política (13)** e, em seguida, selecione as permissões **Policy.Read.All**  e **Policy.ReadWrite.ApplicationConfiguration**.</span><span class="sxs-lookup"><span data-stu-id="6e66f-121">Continue to and expand **Policy (13)**, and then select the **Policy.Read.All**  and **Policy.ReadWrite.ApplicationConfiguration** permissions.</span></span> <span data-ttu-id="6e66f-122">Por fim, role e expanda **Usuários (8)** e selecione **User.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="6e66f-122">Finally, scroll to and expand **Users (8)**, and then select **User.ReadWrite.All**.</span></span>

    ![Rolar e selecionar as permissões approleassignment, application e policy ](./images/application-saml-sso-configure-api/select-permissions.png)

5. <span data-ttu-id="6e66f-124">Selecione **Consentimento** e, em seguida, selecione **Aceitar** para aceitar o consentimento das permissões.</span><span class="sxs-lookup"><span data-stu-id="6e66f-124">Select **Consent**, and then select **Accept** to accept the consent of the permissions.</span></span> <span data-ttu-id="6e66f-125">Você não precisa consentir em nome da organização para essas permissões.</span><span class="sxs-lookup"><span data-stu-id="6e66f-125">You do not need to consent on behalf of your organization for these permissions.</span></span>

    ![Aceitar o consentimento das permissões](./images/application-saml-sso-configure-api/accept-permissions.png)

## <a name="step-1-create-the-application"></a><span data-ttu-id="6e66f-127">Etapa 1: Criar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e66f-127">Step 1: Create the application</span></span>

<span data-ttu-id="6e66f-128">O Azure AD tem uma galeria que contém milhares de aplicativos pré-integrados que você pode usar como modelo para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6e66f-128">Azure AD has a gallery that contains thousands of pre-integrated applications that you can use as a template for your application.</span></span> <span data-ttu-id="6e66f-129">O modelo de aplicativo descreve os metadados para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6e66f-129">The application template describes the metadata for that application.</span></span> <span data-ttu-id="6e66f-130">Usando esse modelo, você pode criar uma instância do aplicativo e da entidade de serviço no locatário para gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="6e66f-130">Using this template, you can create an instance of the application and service principal in your tenant for management.</span></span> 

<span data-ttu-id="6e66f-131">Para criar o aplicativo a partir da galeria, primeiro obtenha o identificador do modelo de aplicativo e, em seguida, use esse identificador para criar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6e66f-131">To create the application from the gallery, you first get the identifier of the application template and then use that identifier to create the application.</span></span>

### <a name="retrieve-the-gallery-application-template-identifier"></a><span data-ttu-id="6e66f-132">Recuperar o identificador do modelo de aplicativo da galeria</span><span class="sxs-lookup"><span data-stu-id="6e66f-132">Retrieve the gallery application template identifier</span></span>

 <span data-ttu-id="6e66f-133">Neste tutorial, recupere o identificador do modelo de aplicativo para `AWS Single Sign-on`.</span><span class="sxs-lookup"><span data-stu-id="6e66f-133">In this tutorial, you retrieve the identifier of the application template for `AWS Single Sign-on`.</span></span> <span data-ttu-id="6e66f-134">Registre o valor da propriedade **id** para usar posteriormente neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="6e66f-134">Record the value of the **id** property to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="6e66f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66f-135">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/applicationTemplates?$filter=displayName eq 'AWS Single Sign-on'
```

#### <a name="response"></a><span data-ttu-id="6e66f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e66f-136">Response</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applicationTemplates",
  "value": [
    {
      "id": "21ed01d2-ec13-4e9e-86c1-cd546719ebc4",
      "displayName": "AWS Single Sign-on",
      "homePageUrl": "https://aws.amazon.com/",
      "supportedSingleSignOnModes": [
        "saml",
        "external"
      ],
      "supportedProvisioningTypes": [
        "sync"
      ],
      "logoUrl": "https://az495088.vo.msecnd.net/app-logo/awssinglesignon_215.png",
      "categories": [
        "developerServices",
        "itInfrastructure",
        "security",
        "New"
      ],
      "publisher": "Amazon Web Services, Inc.",
      "description": "Federate once to AWS SSO & use it to manage access centrally to multiple AWS accounts. Provision users via SCIM & get Azure AD single sign-in access to the AWS Console, CLI, & AWS SSO integrated apps."
    }
  ]
}
```

### <a name="create-the-application"></a><span data-ttu-id="6e66f-137">Criar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e66f-137">Create the application</span></span>

<span data-ttu-id="6e66f-138">Usando o valor **id** registrado para o modelo de aplicativo, crie uma instância do aplicativo e da entidade de serviço no locatário.</span><span class="sxs-lookup"><span data-stu-id="6e66f-138">Using the **id** value that you recorded for the application template, create an instance of the application and service principal in your tenant.</span></span> <span data-ttu-id="6e66f-139">Registre o valor da propriedade **id** do aplicativo e o valor da propriedade **id** para o principal de serviço usar posteriormente neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="6e66f-139">Record the value of the **id** property of the application and the value of the **id** property for the service principal to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="6e66f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66f-140">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/applicationTemplates/21ed01d2-ec13-4e9e-86c1-cd546719ebc4/instantiate
Content-type: application/json

{
  "displayName": "AWS Contoso"
}
```

> [!NOTE]
> <span data-ttu-id="6e66f-141">Aguarde algum tempo para que o aplicativo seja provisionado em seu locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6e66f-141">Allow some time for the app to be provisioned into your Azure AD tenant.</span></span> <span data-ttu-id="6e66f-142">Não é instantâneo.</span><span class="sxs-lookup"><span data-stu-id="6e66f-142">It is not instant.</span></span> <span data-ttu-id="6e66f-143">Uma estratégia é fazer uma consulta GET sobre o objeto de aplicativo e a entidade de serviço a cada 5-10 segundos até que a consulta seja bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="6e66f-143">One strategy is to do a GET query on the application or service principal object every 5-10 seconds until the query is successful.</span></span>

#### <a name="response"></a><span data-ttu-id="6e66f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e66f-144">Response</span></span>

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.applicationServicePrincipal",
  "application": {
    "id": "a9be408a-6c31-4141-8cea-52fcd4a61be8",
    "appId": "17cad0e7-cd2b-4e51-a75d-ba810f3e4045",
    "applicationTemplateId": "21ed01d2-ec13-4e9e-86c1-cd546719ebc4",
    "createdDateTime": "2021-05-10T20:12:03Z",
    "deletedDateTime": null,
    "displayName": "AWS Contoso",
    "groupMembershipClaims": null,
    "identifierUris": [],
    "isFallbackPublicClient": false,
    "signInAudience": "AzureADMyOrg",
    "tags": [],
    "tokenEncryptionKeyId": null,
    "defaultRedirectUri": null,
    "optionalClaims": null,
    "verifiedPublisher": {
      "displayName": null,
      "verifiedPublisherId": null,
      "addedDateTime": null
    },
    "addIns": [],
    "api": {
      "acceptMappedClaims": null,
      "knownClientApplications": [],
      "requestedAccessTokenVersion": null,
      "oauth2PermissionScopes": [
        {
          "adminConsentDescription": "Allow the application to access AWS Contoso on behalf of the signed-in user.",
          "adminConsentDisplayName": "Access AWS Contoso",
          "id": "6f891cd3-c132-4822-930b-f343b4515d19",
          "isEnabled": true,
          "type": "User",
          "userConsentDescription": "Allow the application to access AWS Contoso on your behalf.",
          "userConsentDisplayName": "Access AWS Contoso",
          "value": "user_impersonation"
        }
      ],
      "preAuthorizedApplications": []
    },
    "appRoles": [
      {
        "allowedMemberTypes": [
          "User"
        ],
        "displayName": "User",
        "id": "8774f594-1d59-4279-b9d9-59ef09a23530",
        "isEnabled": true,
        "description": "User",
        "value": null,
        "origin": "Application"
      },
      {
        "allowedMemberTypes": [
          "User"
        ],
        "displayName": "msiam_access",
        "id": "e7f1a7f3-9eda-48e0-9963-bd67bf531afd",
        "isEnabled": true,
        "description": "msiam_access",
        "value": null,
        "origin": "Application"
      }
    ],
    "info": {
      "logoUrl": null,
      "marketingUrl": null,
      "privacyStatementUrl": null,
      "supportUrl": null,
      "termsOfServiceUrl": null
    },
    "keyCredentials": [],
    "parentalControlSettings": {
      "countriesBlockedForMinors": [],
      "legalAgeGroupRule": "Allow"
    },
    "passwordCredentials": [],
    "publicClient": {
      "redirectUris": []
    },
    "requiredResourceAccess": [],
    "web": {
      "homePageUrl": "https://*.signin.aws.amazon.com/platform/saml/acs/*?metadata=awssinglesignon|ISV9.1|primary|z",
      "redirectUris": []
    }
  },
  "servicePrincipal": {
    "id": "a750f6cf-2319-464a-bcc3-456926736a91",
    "deletedDateTime": null,
    "accountEnabled": true,
    "appId": "17cad0e7-cd2b-4e51-a75d-ba810f3e4045",
    "applicationTemplateId": "21ed01d2-ec13-4e9e-86c1-cd546719ebc4",
    "appDisplayName": "AWS Contoso",
    "alternativeNames": [],
    "appOwnerOrganizationId": "8500cad3-193d-48a6-8d00-c129b114dc10",
    "displayName": "AWS Contoso",
    "appRoleAssignmentRequired": true,
    "loginUrl": null,
    "logoutUrl": null,
    "homepage": "https://*.signin.aws.amazon.com/platform/saml/acs/*?metadata=awssinglesignon|ISV9.1|primary|z",
    "notificationEmailAddresses": [],
    "preferredSingleSignOnMode": null,
    "preferredTokenSigningKeyThumbprint": null,
    "replyUrls": [],
    "servicePrincipalNames": [
      "17cad0e7-cd2b-4e51-a75d-ba810f3e4045"
    ],
    "servicePrincipalType": "Application",
    "tags": [
      "WindowsAzureActiveDirectoryIntegratedApp"
    ],
    "tokenEncryptionKeyId": null,
    "samlSingleSignOnSettings": null,
    "verifiedPublisher": {
      "displayName": null,
      "verifiedPublisherId": null,
      "addedDateTime": null
    },
    "addIns": [],
    "appRoles": [
      {
        "allowedMemberTypes": [
          "User"
        ],
        "displayName": "User",
        "id": "8774f594-1d59-4279-b9d9-59ef09a23530",
        "isEnabled": true,
        "description": "User",
        "value": null,
        "origin": "Application"
      },
      {
        "allowedMemberTypes": [
          "User"
        ],
        "displayName": "msiam_access",
        "id": "e7f1a7f3-9eda-48e0-9963-bd67bf531afd",
        "isEnabled": true,
        "description": "msiam_access",
        "value": null,
        "origin": "Application"
      }
    ],
    "info": {
      "logoUrl": null,
      "marketingUrl": null,
      "privacyStatementUrl": null,
      "supportUrl": null,
      "termsOfServiceUrl": null
    },
    "keyCredentials": [],
    "oauth2PermissionScopes": [
      {
        "adminConsentDescription": "Allow the application to access AWS Contoso on behalf of the signed-in user.",
        "adminConsentDisplayName": "Access AWS Contoso",
        "id": "6f891cd3-c132-4822-930b-f343b4515d19",
        "isEnabled": true,
        "type": "User",
        "userConsentDescription": "Allow the application to access AWS Contoso on your behalf.",
        "userConsentDisplayName": "Access AWS Contoso",
        "value": "user_impersonation"
      }
    ],
    "passwordCredentials": []
  }
}
```

## <a name="step-2-configure-single-sign-on"></a><span data-ttu-id="6e66f-145">2. Configurar o logon único</span><span class="sxs-lookup"><span data-stu-id="6e66f-145">Step 2: Configure single sign-on</span></span>

<span data-ttu-id="6e66f-146">Neste tutorial, defina `saml` como modo de logon único na entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="6e66f-146">In this tutorial, you set `saml` as the single sign-on mode in the service principal.</span></span> <span data-ttu-id="6e66f-147">Use o **id** do principal de serviço que você registrou anteriormente.</span><span class="sxs-lookup"><span data-stu-id="6e66f-147">Use the **id** for the service principal that you recorded earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="6e66f-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66f-148">Request</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91
Content-type: servicePrincipal/json

{
  "preferredSingleSignOnMode": "saml"
}
```

#### <a name="response"></a><span data-ttu-id="6e66f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e66f-149">Response</span></span>

```http
HTTP/1.1 204
```

### <a name="set-basic-saml-urls"></a><span data-ttu-id="6e66f-150">Definir URLs básicas de SAML</span><span class="sxs-lookup"><span data-stu-id="6e66f-150">Set basic SAML URLs</span></span>

<span data-ttu-id="6e66f-151">Usando o **id** para o aplicativo que você registrou anteriormente, defina o URI do identificador e redirecione o URI para a AWS no objeto do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6e66f-151">Using the **id** for the application that you recorded earlier, set the identifier URI and redirect URI for AWS in the application object.</span></span>

#### <a name="request"></a><span data-ttu-id="6e66f-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66f-152">Request</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/applications/a9be408a-6c31-4141-8cea-52fcd4a61be8
Content-type: applications/json

{
  "web": {
    "redirectUris": [
      "https://signin.aws.amazon.com/saml"
    ] 
  },
  "identifierUris": [
    "https://signin.aws.amazon.com/saml"
  ]    
}
```

#### <a name="response"></a><span data-ttu-id="6e66f-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e66f-153">Response</span></span>

```http
HTTP/1.1 204
```

### <a name="add-app-roles-optional"></a><span data-ttu-id="6e66f-154">Adicionar funções de aplicativo (opcional)</span><span class="sxs-lookup"><span data-stu-id="6e66f-154">Add app roles (Optional)</span></span>

<span data-ttu-id="6e66f-155">Se o aplicativo exigir as informações da função no token, adicione a definição das funções no objeto do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6e66f-155">If the application requires the role information in the token, add the definition of the roles in the application object.</span></span> 

> [!NOTE] 
> <span data-ttu-id="6e66f-156">Ao adicionar funções de aplicativo, não modifique as funções de aplicativo padrão `msiam_access`.</span><span class="sxs-lookup"><span data-stu-id="6e66f-156">When adding app roles, don't modify the default app roles `msiam_access`.</span></span> 

<span data-ttu-id="6e66f-157">Use o **id** do principal de serviço que você registrou anteriormente.</span><span class="sxs-lookup"><span data-stu-id="6e66f-157">Use the **id** for the service principal that you recorded earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="6e66f-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66f-158">Request</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/serviceprincipals/a9be408a-6c31-4141-8cea-52fcd4a61be8
Content-type: serviceprincipals/json

{
  "appRoles": [
    {
      "allowedMemberTypes": [
        "User"
      ],
      "displayName": "User",
      "id": "8774f594-1d59-4279-b9d9-59ef09a23530",
      "isEnabled": true,
      "description": "User",
      "value": null,
      "origin": "Application"
    },
    {
      "allowedMemberTypes": [
        "User"
      ],
      "displayName": "msiam_access",
      "id": "e7f1a7f3-9eda-48e0-9963-bd67bf531afd",
      "isEnabled": true,
      "description": "msiam_access",
      "value": null,
      "origin": "Application"
    },
    {
      "allowedMemberTypes": [
        "User"
      ],
      "description": "Admin,WAAD",
      "displayName": "Admin,WAAD",
      "id": "3a84e31e-bffa-470f-b9e6-754a61e4dc63",
      "isEnabled": true,
      "value": "arn:aws:iam::212743507312:role/accountname-aws-admin,arn:aws:iam::212743507312:saml-provider/WAAD"
    },
    {
      "allowedMemberTypes": [
        "User"
      ],
      "description": "Finance,WAAD",
      "displayName": "Finance,WAAD",
      "id": "7a960000-ded3-455b-8c04-4f2ace00319b",
      "isEnabled": true,
      "value": "arn:aws:iam::212743507312:role/accountname-aws-finance,arn:aws:iam::212743507312:saml-provider/WAAD"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="6e66f-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e66f-159">Response</span></span>

```http
HTTP/1.1 204
```

## <a name="step-3-configure-claims-mapping"></a><span data-ttu-id="6e66f-160">3. Configurar mapeamento de declarações</span><span class="sxs-lookup"><span data-stu-id="6e66f-160">Step 3: Configure claims mapping</span></span>

### <a name="create-a-claims-mapping-policy"></a><span data-ttu-id="6e66f-161">Criar uma política de mapeamento de declarações</span><span class="sxs-lookup"><span data-stu-id="6e66f-161">Create a claims mapping policy</span></span>

<span data-ttu-id="6e66f-162">Além das declarações básicas, configure as seguintes declarações para o Azure AD emitir no token SAML:</span><span class="sxs-lookup"><span data-stu-id="6e66f-162">In addition to the basic claims, configure the following claims for Azure AD to emit in the SAML token:</span></span>

| <span data-ttu-id="6e66f-163">Nome da declaração</span><span class="sxs-lookup"><span data-stu-id="6e66f-163">Claim name</span></span> | <span data-ttu-id="6e66f-164">Origem</span><span class="sxs-lookup"><span data-stu-id="6e66f-164">Source</span></span>  |
|---------|---------|
| `https://aws.amazon.com/SAML/Attributes/Role` | <span data-ttu-id="6e66f-165">assignedroles</span><span class="sxs-lookup"><span data-stu-id="6e66f-165">assignedroles</span></span>| 
| `https://aws.amazon.com/SAML/Attributes/RoleSessionName` | <span data-ttu-id="6e66f-166">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="6e66f-166">userprincipalname</span></span> |
| `https://aws.amazon.com/SAML/Attributes/SessionDuration` | <span data-ttu-id="6e66f-167">"900"</span><span class="sxs-lookup"><span data-stu-id="6e66f-167">"900"</span></span> |
| <span data-ttu-id="6e66f-168">funções</span><span class="sxs-lookup"><span data-stu-id="6e66f-168">roles</span></span> | <span data-ttu-id="6e66f-169">assignedroles</span><span class="sxs-lookup"><span data-stu-id="6e66f-169">assignedroles</span></span> |
| `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier` | <span data-ttu-id="6e66f-170">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="6e66f-170">userprincipalname</span></span> |

> [!NOTE]
> <span data-ttu-id="6e66f-171">Algumas chaves na política de mapeamento de declarações são sensíveis a letras maiúsculas e minúsculas (por exemplo, "Version").</span><span class="sxs-lookup"><span data-stu-id="6e66f-171">Some keys in the claims mapping policy are case sensitive (for example, "Version").</span></span> <span data-ttu-id="6e66f-172">Se você receber uma mensagem de erro como "A propriedade tem um valor inválido", isso poderia ser um problema de diferenciação de maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="6e66f-172">If you receive an error message such as "Property has an invalid value", it might be a case sensitive issue.</span></span>

<span data-ttu-id="6e66f-173">Crie a política de mapeamento de declarações e registre o valor da propriedade **id** para usar posteriormente neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="6e66f-173">Create the claims mapping policy and record the value of the **id** property to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="6e66f-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66f-174">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies
Content-type: claimsMappingPolicies/json

{
  "definition": [
    "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Source\":\"user\",\"ID\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/nameidentifier\"}]}}"
    ],
  "displayName": "AWS Claims Policy",
  "isOrganizationDefault": false
}
```

#### <a name="response"></a><span data-ttu-id="6e66f-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e66f-175">Response</span></span>

```http
HTTP/1.1 201 OK
Content-type: claimsMappingPolicies/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/claimsMappingPolicies/$entity",
  "id": "a4b35718-fd5e-4ca8-8248-a3c9934b1b78",
  "deletedDateTime": null,
  "definition": [
    "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Source\":\"user\",\"ID\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/nameidentifier\"}]}}"
  ],
  "displayName": "AWS Claims Policy",
  "isOrganizationDefault": false
}
```

### <a name="assign-a-claims-mapping-policy-to-a-service-principal"></a><span data-ttu-id="6e66f-176">Atribuir uma política de mapeamento de declarações a uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="6e66f-176">Assign a claims mapping policy to a service principal</span></span>

<span data-ttu-id="6e66f-177">Use o **id** do principal de serviço que você registrou anteriormente para atribuir uma política de mapeamento de declarações a ele.</span><span class="sxs-lookup"><span data-stu-id="6e66f-177">Use the **id** for the service principal that you recorded earlier to assign a claims mapping policy to it.</span></span> <span data-ttu-id="6e66f-178">Use o valor da propriedade **id** para a política de mapeamento de declarações no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e66f-178">Use the value of the **id** property for the claims mapping policy in the body of the request.</span></span>

#### <a name="request"></a><span data-ttu-id="6e66f-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66f-179">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91/claimsMappingPolicies/$ref
Content-type: claimsMappingPolicies/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/a4b35718-fd5e-4ca8-8248-a3c9934b1b78"
}
```

#### <a name="response"></a><span data-ttu-id="6e66f-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e66f-180">Response</span></span>

```http
HTTP/1.1 204
```

## <a name="step-4-configure-a-signing-certificate"></a><span data-ttu-id="6e66f-181">Etapa 4. Configurar um certificado de autenticação</span><span class="sxs-lookup"><span data-stu-id="6e66f-181">Step 4: Configure a signing certificate</span></span>

<span data-ttu-id="6e66f-182">Neste tutorial, você precisa de um certificado autoassinado que o Azure Active Directory pode usar para assinar uma resposta SAML.</span><span class="sxs-lookup"><span data-stu-id="6e66f-182">You need a self-signed certificate that Azure AD can use to sign a SAML response.</span></span> <span data-ttu-id="6e66f-183">Você pode usar seu próprio certificado ou pode usar o exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="6e66f-183">You can use your own certificate or you can use the following example.</span></span> 

### <a name="create-a-signing-certificate"></a><span data-ttu-id="6e66f-184">Criar um certificado de assinatura</span><span class="sxs-lookup"><span data-stu-id="6e66f-184">Create a signing certificate</span></span>

<span data-ttu-id="6e66f-185">Usando o **id** do principal de serviço que você criou, crie um novo certificado e inclua-o no principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="6e66f-185">Using the **id** of the service principal that you created, create a new certificate and add it to the service principal.</span></span>

#### <a name="request"></a><span data-ttu-id="6e66f-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66f-186">Request</span></span>

```http
POST https://graph.microsoft.com/beta/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91/addTokenSigningCertificate
Content-type: application/json

{
    "displayName":"CN=AWSContoso",
    "endDateTime":"2024-01-25T00:00:00Z"
}
```

#### <a name="response"></a><span data-ttu-id="6e66f-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e66f-187">Response</span></span>

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.selfSignedCertificate",
  "customKeyIdentifier": "p9PEYmuKhP2oaMzGfSdNQC/9ChA=",
  "displayName": "CN=AWSContoso",
  "endDateTime": "2024-01-25T00:00:00Z",
  "key": "MIICqjCCAZKgAwIBAgIId....4rnrk43wp75yqjRbOhAZ1ExAxVqW+o2JslhjUeltUMNQW+ynOfs9oHu1ZdnGmxrE=",
  "keyId": "70883316-50be-4016-ba80-19d9fbad873d",
  "startDateTime": "2021-05-10T20:35:37.5754318Z",
  "thumbprint": "A7D3C4626B8A84FDA868CCC67D274D402FFD0A10",
  "type": "AsymmetricX509Cert",
  "usage": "Verify"
}
```

### <a name="activate-the-custom-signing-key"></a><span data-ttu-id="6e66f-188">Adicionar a chave de assinatura personalizada</span><span class="sxs-lookup"><span data-stu-id="6e66f-188">Activate the custom signing key</span></span>

<span data-ttu-id="6e66f-189">É necessário definir a propriedade **preferredTokenSigningKeyThumbprint** da entidade de serviço para a impressão digital do certificado que você deseja que o Azure AD use para assinar a resposta SAML.</span><span class="sxs-lookup"><span data-stu-id="6e66f-189">You need to set the **preferredTokenSigningKeyThumbprint** property of the service principal to the thumbprint of the certificate that you want Azure AD to use to sign the SAML response.</span></span> 

#### <a name="request"></a><span data-ttu-id="6e66f-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66f-190">Request</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91
Content-type: servicePrincipals/json

{
  "preferredTokenSigningKeyThumbprint": "A7D3C4626B8A84FDA868CCC67D274D402FFD0A10"
}
```

#### <a name="response"></a><span data-ttu-id="6e66f-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e66f-191">Response</span></span>

```http
HTTP/1.1 204
```

## <a name="step-5-assign-users"></a><span data-ttu-id="6e66f-192">Etapa 5. Atribuir usuários</span><span class="sxs-lookup"><span data-stu-id="6e66f-192">Step 5: Assign users</span></span>

### <a name="create-a-user-account"></a><span data-ttu-id="6e66f-193">Criar uma conta de usuário</span><span class="sxs-lookup"><span data-stu-id="6e66f-193">Create a user account</span></span>

<span data-ttu-id="6e66f-194">Para este tutorial, crie uma conta de usuário que será adicionada ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6e66f-194">For this tutorial, you create a user account that is added to the application.</span></span> <span data-ttu-id="6e66f-195">No corpo da solicitação, altere contoso.com para o nome de domínio do seu locatário.</span><span class="sxs-lookup"><span data-stu-id="6e66f-195">In the request body, change contoso.com to the domain name of your tenant.</span></span> <span data-ttu-id="6e66f-196">Encontre informações sobre locatários na página de visão geral do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6e66f-196">You can find tenant information on the Azure Active Directory overview page.</span></span> <span data-ttu-id="6e66f-197">Registre o **id** do usuário a ser usado posteriormente neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="6e66f-197">Record the **id** of the user to be used later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="6e66f-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66f-198">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled":true,
  "displayName":"MyTestUser1",
  "mailNickname":"MyTestUser1",
  "userPrincipalName":"MyTestUser1@contoso.com",
  "passwordProfile": {
    "forceChangePasswordNextSignIn":true,
    "password":"Contoso1234"
  }
}
```

#### <a name="response"></a><span data-ttu-id="6e66f-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e66f-199">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "040f9599-7c0f-4f94-aa75-8394c4c6ea9b",
  "businessPhones": [],
  "displayName": "MyTestUser1",
  "givenName": null,
  "jobTitle": null,
  "mail": null,
  "mobilePhone": null,
  "officeLocation": null,
  "preferredLanguage": null,
  "surname": null,
  "userPrincipalName": "MyTestUser1@contoso.com"
}
```

### <a name="assign-a-user-to-the-application"></a><span data-ttu-id="6e66f-200">Atribuir um usuário ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e66f-200">Assign a user to the application</span></span>

<span data-ttu-id="6e66f-201">Atribua o usuário que você criou à entidade de serviço e atribua a função de aplicativo `Admin,WAAD`.</span><span class="sxs-lookup"><span data-stu-id="6e66f-201">Assign the user that you created to the service principal and assign the `Admin,WAAD` app role.</span></span> 

<span data-ttu-id="6e66f-202">No corpo da solicitação, forneça estes valores:</span><span class="sxs-lookup"><span data-stu-id="6e66f-202">In the request body, provide these values:</span></span>

- <span data-ttu-id="6e66f-203">**principalId** – O **id** da conta de usuário que você criou.</span><span class="sxs-lookup"><span data-stu-id="6e66f-203">**principalId** - The **id** of the user account that you created.</span></span>
- <span data-ttu-id="6e66f-204">**appRoleId** – O **id** da função de apĺicativo `Admin,WAAD` que você adicionou.</span><span class="sxs-lookup"><span data-stu-id="6e66f-204">**appRoleId** - The **id** of the `Admin,WAAD` app role that you added.</span></span>
- <span data-ttu-id="6e66f-205">**resourceId** – A **id** da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="6e66f-205">**resourceId** - The **id** of the service principal.</span></span>

#### <a name="request"></a><span data-ttu-id="6e66f-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66f-206">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91/appRoleAssignments
Content-type: appRoleAssignments/json

{
  "principalId": "040f9599-7c0f-4f94-aa75-8394c4c6ea9b",
  "principalType": "User",
  "appRoleId":"3a84e31e-bffa-470f-b9e6-754a61e4dc63",
  "resourceId":"a750f6cf-2319-464a-bcc3-456926736a91"
}
```

#### <a name="response"></a><span data-ttu-id="6e66f-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e66f-207">Response</span></span>

```http
HTTP/1.1 201 
Content-type: appRoleAssignments/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals('a750f6cf-2319-464a-bcc3-456926736a91')/appRoleAssignments/$entity",
  "id": "mZUPBA98lE-qdYOUxMbqm2qY3odGRGdFtpYJkAfUC0Q",
  "deletedDateTime": null,
  "appRoleId": "3a84e31e-bffa-470f-b9e6-754a61e4dc63",
  "createdDateTime": "2021-05-10T21:04:11.0480851Z",
  "principalDisplayName": "MyTestUser1",
  "principalId": "040f9599-7c0f-4f94-aa75-8394c4c6ea9b",
  "principalType": "User",
  "resourceDisplayName": "AWS Contoso",
  "resourceId": "a750f6cf-2319-464a-bcc3-456926736a91"
}
```

## <a name="step-6-get-azure-ad-saml-metadata"></a><span data-ttu-id="6e66f-208">Etapa 6: Obter metadados SAML do Azure AD</span><span class="sxs-lookup"><span data-stu-id="6e66f-208">Step 6: Get Azure AD SAML metadata</span></span>

<span data-ttu-id="6e66f-209">Use a URL a seguir para obter os metadados do SAML do Azure AD para o aplicativo específico configurado.</span><span class="sxs-lookup"><span data-stu-id="6e66f-209">Use the following URL to get the Azure AD SAML metadata for the specific configured application.</span></span> <span data-ttu-id="6e66f-210">Os metadados contêm informações como o certificado de assinatura, o Azure AD entityID e o Azure AD SingleSignOnService, entre outras.</span><span class="sxs-lookup"><span data-stu-id="6e66f-210">The metadata contains information such as the signing certificate, Azure AD entityID, and Azure AD SingleSignOnService, among others.</span></span>

`https://login.microsoftonline.com/{tenant-id}/federationmetadata/2007-06/federationmetadata.xml?appid={app-id}`

<span data-ttu-id="6e66f-211">A seguir, é possível ver um exemplo do que você pode ver no aplicativo:</span><span class="sxs-lookup"><span data-stu-id="6e66f-211">The following shows an example of what you might see for your application:</span></span>

```
<EntityDescriptor xmlns="urn:oasis:names:tc:SAML:2.0:metadata" ID="_05fbbf53-e892-43c9-9300-1f6738ace02c" entityID="https://sts.windows.net/2f82f566-5953-43f4-9251-79c6009bdf24/">
<Signature xmlns="http://www.w3.org/2000/09/xmldsig#">

...

<SingleLogoutService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect" Location="https://login.microsoftonline.com/2f82f566-5953-43f4-9251-79c6009bdf24/saml2"/>
<SingleSignOnService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect" Location="https://login.microsoftonline.com/2f82f566-5953-43f4-9251-79c6009bdf24/saml2"/>
<SingleSignOnService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST" Location="https://login.microsoftonline.com/2f82f566-5953-43f4-9251-79c6009bdf24/saml2"/>
</IDPSSODescriptor>
</EntityDescriptor>
```

## <a name="step-7-clean-up-resources"></a><span data-ttu-id="6e66f-212">Etapa 7: Limpar recursos</span><span class="sxs-lookup"><span data-stu-id="6e66f-212">Step 7: Clean up resources</span></span>

<span data-ttu-id="6e66f-213">Nessa etapa, remova os recursos que criou.</span><span class="sxs-lookup"><span data-stu-id="6e66f-213">In this step, you remove the resources that you created.</span></span>


### <a name="delete-the-application"></a><span data-ttu-id="6e66f-214">Excluir o aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e66f-214">Delete the application</span></span>

<span data-ttu-id="6e66f-215">Exclua o aplicativo que você criou.</span><span class="sxs-lookup"><span data-stu-id="6e66f-215">Delete the application that you created.</span></span>

#### <a name="request"></a><span data-ttu-id="6e66f-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66f-216">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/applications/a9be408a-6c31-4141-8cea-52fcd4a61be8
```

#### <a name="response"></a><span data-ttu-id="6e66f-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e66f-217">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-user-account"></a><span data-ttu-id="6e66f-218">Excluir a conta de usuário</span><span class="sxs-lookup"><span data-stu-id="6e66f-218">Delete the user account</span></span>

<span data-ttu-id="6e66f-219">Exclua a conta de usuário MyTestUser1.</span><span class="sxs-lookup"><span data-stu-id="6e66f-219">Delete the MyTestUser1 user account.</span></span>

#### <a name="request"></a><span data-ttu-id="6e66f-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66f-220">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/users/040f9599-7c0f-4f94-aa75-8394c4c6ea9b
```

#### <a name="response"></a><span data-ttu-id="6e66f-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e66f-221">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-claims-mapping-policy"></a><span data-ttu-id="6e66f-222">Excluir a política de mapeamento de declarações</span><span class="sxs-lookup"><span data-stu-id="6e66f-222">Delete the claims mapping policy</span></span>

<span data-ttu-id="6e66f-223">Exclua a política de mapeamento de declarações.</span><span class="sxs-lookup"><span data-stu-id="6e66f-223">Delete the claims mapping policy.</span></span>

#### <a name="request"></a><span data-ttu-id="6e66f-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66f-224">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/a4b35718-fd5e-4ca8-8248-a3c9934b1b78
```

#### <a name="response"></a><span data-ttu-id="6e66f-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e66f-225">Response</span></span>

```http
No Content - 204
```

## <a name="see-also"></a><span data-ttu-id="6e66f-226">Confira também</span><span class="sxs-lookup"><span data-stu-id="6e66f-226">See also</span></span>

- <span data-ttu-id="6e66f-227">No AWS, você pode [habilitar o provisionamento de usuário](/azure/active-directory/app-provisioning/application-provisioning-configure-api) para buscar todas as funções dessa conta do AWS.</span><span class="sxs-lookup"><span data-stu-id="6e66f-227">For AWS, you can [enable user provisioning](/azure/active-directory/app-provisioning/application-provisioning-configure-api) to fetch all the roles from that AWS account.</span></span> <span data-ttu-id="6e66f-228">Para saber mais, confira [Configurar a declaração de função emitida no token SAML](/azure/active-directory/develop/active-directory-enterprise-app-role-management).</span><span class="sxs-lookup"><span data-stu-id="6e66f-228">For more information, see [Configure the role claim issued in the SAML token](/azure/active-directory/develop/active-directory-enterprise-app-role-management).</span></span>
- <span data-ttu-id="6e66f-229">[Personalizar as declarações emitidas em tokens para um aplicativo específico em um locatário](/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="6e66f-229">[Customize claims emitted in tokens for a specific app in a tenant](/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
- <span data-ttu-id="6e66f-230">Você pode usar a API applicationTemplate para criar uma instância [Aplicativos inexistentes na galeria](/azure/active-directory/manage-apps/view-applications-portal).</span><span class="sxs-lookup"><span data-stu-id="6e66f-230">You can use the applicationTemplate API to instantiate [Non-Gallery apps](/azure/active-directory/manage-apps/view-applications-portal).</span></span> <span data-ttu-id="6e66f-231">Use applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span><span class="sxs-lookup"><span data-stu-id="6e66f-231">Use applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>
- [<span data-ttu-id="6e66f-232">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="6e66f-232">applicationTemplate</span></span>](/graph/api/resources/applicationtemplate)
- [<span data-ttu-id="6e66f-233">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6e66f-233">appRoleAssignment</span></span>](/graph/api/resources/approleassignment)
- [<span data-ttu-id="6e66f-234">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="6e66f-234">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal)
- [<span data-ttu-id="6e66f-235">application</span><span class="sxs-lookup"><span data-stu-id="6e66f-235">application</span></span>](/graph/api/resources/application)
- [<span data-ttu-id="6e66f-236">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="6e66f-236">claimsMappingPolicy</span></span>](/graph/api/resources/claimsmappingpolicy)
- [<span data-ttu-id="6e66f-237">keyCredential</span><span class="sxs-lookup"><span data-stu-id="6e66f-237">keyCredential</span></span>](/graph/api/resources/keycredential)
- [<span data-ttu-id="6e66f-238">addTokenSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="6e66f-238">addTokenSigningCertificate</span></span>](/graph/api/serviceprincipal-addtokensigningcertificate?view=graph-rest-beta&preserve-view=true)

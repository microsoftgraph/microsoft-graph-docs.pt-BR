---
title: Criar aplicativo
description: Crie um novo aplicativo.
author: davidmu1
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b4c0401342c3bf40cd7018542ece48c9c91a64f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939695"
---
# <a name="create-application"></a><span data-ttu-id="f1b8a-103">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1b8a-103">Create application</span></span>

<span data-ttu-id="f1b8a-104">Crie um novo objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="f1b8a-104">[Create a new application pool](../resources/application.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="f1b8a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1b8a-105">Permissions</span></span>
<span data-ttu-id="f1b8a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1b8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f1b8a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1b8a-108">Permission type</span></span>      | <span data-ttu-id="f1b8a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1b8a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1b8a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1b8a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f1b8a-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f1b8a-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f1b8a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1b8a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1b8a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-113">Not supported.</span></span>    |
|<span data-ttu-id="f1b8a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1b8a-114">Application</span></span> | <span data-ttu-id="f1b8a-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1b8a-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1b8a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1b8a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="f1b8a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1b8a-117">Request headers</span></span>
| <span data-ttu-id="f1b8a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f1b8a-118">Name</span></span>       | <span data-ttu-id="f1b8a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1b8a-119">Type</span></span> | <span data-ttu-id="f1b8a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1b8a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f1b8a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1b8a-121">Authorization</span></span>  | <span data-ttu-id="f1b8a-122">string</span><span class="sxs-lookup"><span data-stu-id="f1b8a-122">string</span></span>  | <span data-ttu-id="f1b8a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1b8a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1b8a-125">Request body</span></span>
<span data-ttu-id="f1b8a-126">No corpo da solicitação, forneça uma representação JSON do objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="f1b8a-126">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span> <span data-ttu-id="f1b8a-127">O corpo da solicitação deve conter **displayName**, que é uma propriedade obrigatória.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-127">The request body must contain  **displayName**, which is a required property.</span></span>

## <a name="response"></a><span data-ttu-id="f1b8a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1b8a-128">Response</span></span>

<span data-ttu-id="f1b8a-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-129">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f1b8a-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f1b8a-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="f1b8a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1b8a-131">Request</span></span>
<span data-ttu-id="f1b8a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_application_from_applications"
}-->
```http
POST https://graph.microsoft.com/v1.0/applications
Content-type: application/json
Content-length: 67

{
  "displayName": "Display name"
}
```

### <a name="response"></a><span data-ttu-id="f1b8a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1b8a-133">Response</span></span>
<span data-ttu-id="f1b8a-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="f1b8a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 1145

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications/$entity",
    "id": "03ef14b0-ca33-4840-8f4f-d6e91916010e",
    "deletedDateTime": null,
    "isFallbackPublicClient": null,
    "appId": "631a96bc-a705-4eda-9f99-fdaf9f54f6a2",
    "applicationTemplateId": null,
    "identifierUris": [],
    "createdDateTime": "2019-09-17T19:10:35.2742618Z",
    "displayName": "Display name",
    "isDeviceOnlyAuthSupported": null,
    "groupMembershipClaims": null,
    "optionalClaims": null,
    "addIns": [],
    "publisherDomain": "contoso.onmicrosoft.com",
    "signInAudience": "AzureADandPersonalMicrosoftAccount",
    "tags": [],
    "tokenEncryptionKeyId": null,
    "api": {
        "requestedAccessTokenVersion": 2,
        "acceptMappedClaims": null,
        "knownClientApplications": [],
        "oauth2PermissionScopes": [],
        "preAuthorizedApplications": []
    },
    "appRoles": [],
    "publicClient": {
        "redirectUris": []
    },
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "parentalControlSettings": {
        "countriesBlockedForMinors": [],
        "legalAgeGroupRule": "Allow"
    },
    "passwordCredentials": [],
    "requiredResourceAccess": [],
    "web": {
        "redirectUris": [],
        "homePageUrl": null,
        "logoutUrl": null,
        "implicitGrantSettings": {
            "enableIdTokenIssuance": false,
            "enableAccessTokenIssuance": false
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

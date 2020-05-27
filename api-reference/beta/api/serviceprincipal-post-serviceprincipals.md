---
title: Criar o servicePrincipalName
description: Criar um novo objeto servicePrincipalName.
author: sureshja
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4e5548d375ea27197a40ddb9cd61ec2d8463103d
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44382633"
---
# <a name="create-serviceprincipal"></a><span data-ttu-id="862a4-103">Criar o servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="862a4-103">Create servicePrincipal</span></span>

<span data-ttu-id="862a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="862a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="862a4-105">Criar um novo objeto [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="862a4-105">Create a new [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="862a4-106">A adição de [**passwordCredential**](../resources/passwordcredential.md) ao criar o servicePrincipalName não é suportada.</span><span class="sxs-lookup"><span data-stu-id="862a4-106">Adding [**passwordCredential**](../resources/passwordcredential.md) when creating servicePrincipals is not supported.</span></span> <span data-ttu-id="862a4-107">Use o método [addpassword](serviceprincipal-addpassword.md) para adicionar senhas para um servicePrincipalName.</span><span class="sxs-lookup"><span data-stu-id="862a4-107">Use the [addPassword](serviceprincipal-addpassword.md) method to add passwords for a servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="862a4-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="862a4-108">Permissions</span></span>
<span data-ttu-id="862a4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="862a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="862a4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="862a4-111">Permission type</span></span>      | <span data-ttu-id="862a4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="862a4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="862a4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="862a4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="862a4-114">Application. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="862a4-114">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="862a4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="862a4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="862a4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="862a4-116">Not supported.</span></span>    |
|<span data-ttu-id="862a4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="862a4-117">Application</span></span> | <span data-ttu-id="862a4-118">Application. ReadWrite. OwnedBy, Application. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="862a4-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="862a4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="862a4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /serviceprincipals
```

## <a name="request-headers"></a><span data-ttu-id="862a4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="862a4-120">Request headers</span></span>
| <span data-ttu-id="862a4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="862a4-121">Name</span></span>       | <span data-ttu-id="862a4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="862a4-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="862a4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="862a4-123">Authorization</span></span> | <span data-ttu-id="862a4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="862a4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="862a4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="862a4-126">Content-Type</span></span> | <span data-ttu-id="862a4-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="862a4-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="862a4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="862a4-129">Request body</span></span>
<span data-ttu-id="862a4-130">No corpo da solicitação, forneça uma representação JSON de um objeto [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="862a4-130">In the request body, supply a JSON representation of a [serviceprincipal](../resources/serviceprincipal.md) object.</span></span> <span data-ttu-id="862a4-131">O corpo da solicitação deve conter **AppID**.</span><span class="sxs-lookup"><span data-stu-id="862a4-131">The request body must contain  **appId**.</span></span>

## <a name="response"></a><span data-ttu-id="862a4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="862a4-132">Response</span></span>

<span data-ttu-id="862a4-133">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [servicePrincipalName](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="862a4-133">If successful, this method returns a `201 Created` response code and a [serviceprincipal](../resources/serviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="862a4-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="862a4-134">Examples</span></span>
### <a name="request"></a><span data-ttu-id="862a4-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="862a4-135">Request</span></span>
<span data-ttu-id="862a4-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="862a4-136">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="862a4-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="862a4-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_serviceprincipal_from_serviceprincipals"
}-->
```http
POST https://graph.microsoft.com/beta/serviceprincipals
Content-type: application/json

{
  "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
}
```
# <a name="c"></a>[<span data-ttu-id="862a4-138">C#</span><span class="sxs-lookup"><span data-stu-id="862a4-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-serviceprincipal-from-serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="862a4-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="862a4-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-serviceprincipal-from-serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="862a4-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="862a4-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-serviceprincipal-from-serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="862a4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="862a4-141">Response</span></span>
<span data-ttu-id="862a4-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="862a4-142">Here is an example of the response.</span></span> 

> <span data-ttu-id="862a4-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="862a4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals/$entity",
    "id": "59e617e5-e447-4adc-8b88-00af644d7c92",
    "deletedDateTime": null,
    "accountEnabled": true,
    "appDisplayName": "My App",
    "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
    "applicationTemplateId": null,
    "appOwnerOrganizationId": "1bc1c026-2f7b-48a5-98da-afa2fd8bc7bc",
    "appRoleAssignmentRequired": false,
    "displayName": "foo",
    "errorUrl": null,
    "homepage": null,
    "loginUrl": null,
    "logoutUrl": null,
    "notificationEmailAddresses": [],
    "preferredSingleSignOnMode": null,
    "preferredTokenSigningKeyEndDateTime": null,
    "preferredTokenSigningKeyThumbprint": null,
    "publisherName": "Contoso",
    "replyUrls": [],
    "samlMetadataUrl": null,
    "samlSingleSignOnSettings": null,
    "servicePrincipalNames": [
        "f1bd758f-4a1a-4b71-aa20-a248a22a8928"
    ],
    "signInAudience": "AzureADandPersonalMicrosoftAccount",
    "tags": [],
    "addIns": [],
    "api": {
        "resourceSpecificApplicationPermissions": []
    },
    "appRoles": [],
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "publishedPermissionScopes": [],
    "passwordCredentials": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

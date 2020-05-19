---
title: Obter um servicePrincipal
description: Recuperar as propriedades e as relações do objeto serviceprincipal.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f111552f6885fa514a003ccd37c3eb157035a33d
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291262"
---
# <a name="get-serviceprincipal"></a><span data-ttu-id="00cc6-103">Obter um servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="00cc6-103">Get servicePrincipal</span></span>

<span data-ttu-id="00cc6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00cc6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00cc6-105">Recupere as propriedades e os relacionamentos de um objeto [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="00cc6-105">Retrieve the properties and relationships of a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="00cc6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="00cc6-106">Permissions</span></span>
<span data-ttu-id="00cc6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00cc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="00cc6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00cc6-109">Permission type</span></span>      | <span data-ttu-id="00cc6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00cc6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00cc6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00cc6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="00cc6-112">Application. Read. All, Directory. Read. All, Application. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="00cc6-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="00cc6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00cc6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00cc6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00cc6-114">Not supported.</span></span>    |
|<span data-ttu-id="00cc6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00cc6-115">Application</span></span> | <span data-ttu-id="00cc6-116">Application. Read. All, Directory. Read. All, Application. ReadWrite. OwnedBy, Application. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="00cc6-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00cc6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00cc6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00cc6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="00cc6-118">Optional query parameters</span></span>
<span data-ttu-id="00cc6-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="00cc6-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00cc6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00cc6-120">Request headers</span></span>
| <span data-ttu-id="00cc6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="00cc6-121">Name</span></span>           | <span data-ttu-id="00cc6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="00cc6-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="00cc6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="00cc6-123">Authorization</span></span>  | <span data-ttu-id="00cc6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00cc6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="00cc6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00cc6-126">Request body</span></span>
<span data-ttu-id="00cc6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="00cc6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00cc6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="00cc6-128">Response</span></span>
<span data-ttu-id="00cc6-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [servicePrincipalName](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00cc6-129">If successful, this method returns a `200 OK` response code and a [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="00cc6-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="00cc6-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="00cc6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00cc6-131">Request</span></span>
<span data-ttu-id="00cc6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00cc6-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}
```

### <a name="response"></a><span data-ttu-id="00cc6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="00cc6-133">Response</span></span>
<span data-ttu-id="00cc6-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00cc6-134">Here is an example of the response.</span></span> 

><span data-ttu-id="00cc6-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00cc6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
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
  "description": "Get servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
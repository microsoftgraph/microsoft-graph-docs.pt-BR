---
title: Obter um servicePrincipal
description: Recuperar as propriedades e as relações do objeto serviceprincipal.
author: sureshja
localization_priority: Priority
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 70b8802cb25cd7d731d48d5eededaaf188204155
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813038"
---
# <a name="get-serviceprincipal"></a><span data-ttu-id="c0019-103">Obter um servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="c0019-103">Get servicePrincipal</span></span>

<span data-ttu-id="c0019-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0019-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0019-105">Recuperar as propriedades e as relações de um objeto [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="c0019-105">Retrieve the properties and relationships of a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0019-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0019-106">Permissions</span></span>
<span data-ttu-id="c0019-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0019-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0019-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0019-109">Permission type</span></span>      | <span data-ttu-id="c0019-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0019-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0019-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0019-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c0019-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c0019-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c0019-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0019-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0019-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0019-114">Not supported.</span></span>    |
|<span data-ttu-id="c0019-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0019-115">Application</span></span> | <span data-ttu-id="c0019-116">Application.Read.All, Application.ReadWrite.All, Application.ReadWrite.OwnedBy, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0019-116">Application.Read.All, Application.ReadWrite.All, Application.ReadWrite.OwnedBy, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0019-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0019-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0019-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c0019-118">Optional query parameters</span></span>
<span data-ttu-id="c0019-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c0019-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0019-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0019-120">Request headers</span></span>
| <span data-ttu-id="c0019-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c0019-121">Name</span></span>           | <span data-ttu-id="c0019-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0019-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="c0019-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0019-123">Authorization</span></span>  | <span data-ttu-id="c0019-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0019-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0019-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0019-126">Request body</span></span>
<span data-ttu-id="c0019-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0019-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0019-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0019-128">Response</span></span>
<span data-ttu-id="c0019-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0019-129">If successful, this method returns a `200 OK` response code and a [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c0019-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c0019-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="c0019-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0019-131">Request</span></span>
<span data-ttu-id="c0019-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0019-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c0019-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0019-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="c0019-134">C#</span><span class="sxs-lookup"><span data-stu-id="c0019-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0019-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0019-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0019-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0019-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0019-137">Java</span><span class="sxs-lookup"><span data-stu-id="c0019-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c0019-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0019-138">Response</span></span>
<span data-ttu-id="c0019-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0019-139">Here is an example of the response.</span></span> 

><span data-ttu-id="c0019-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c0019-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled": true,
  "addIns": [],
  "alternativeNames": ["http://contoso/a7770d29-4321-41a6-b863-ca11d6639448"],
  "appDisplayName": "My app",
  "appId": "appId-value",
  "appOwnerOrganizationId": "65415bb1-9267-4313-bbf5-ae259732ee12",
  "appRoleAssignmentRequired":true,
  "appRoles": [],
  "disabledByMicrosoftStatus": null,
  "displayName": "My app instance in tenant",
  "endpoints": [],
  "homepage": null,
  "id": "00af5dfb-85da-4b41-a677-0c6b86dd34f8",
  "info": {
    "termsOfServiceUrl": null,
    "supportUrl": null,
    "privacyStatementUrl": null,
    "marketingUrl": null,
    "logoUrl": null
  },
  "keyCredentials": [],
  "logoutUrl": null,
  "oauth2PermissionScopes": [],
  "passwordCredentials": [],
  "publisherName": null,
  "replyUrls": [],
  "servicePrincipalNames": [],
  "servicePrincipalType": null,
  "signInAudience": "AzureADandPersonalMicrosoftAccount",
  "tags": [],
  "tokenEncryptionKeyId": null
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

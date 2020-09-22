---
title: Listar servicePrincipals
description: Recupere uma lista de objetos servicePrincipal.
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 46b14333d100c4c4859690978a39397a2781290c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48045604"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="630cc-103">Listar servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="630cc-103">List servicePrincipals</span></span>

<span data-ttu-id="630cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="630cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="630cc-105">Recupere uma lista de objetos [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="630cc-105">Retrieve a list of [servicePrincipal](../resources/serviceprincipal.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="630cc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="630cc-106">Permissions</span></span>

<span data-ttu-id="630cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="630cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="630cc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="630cc-109">Permission type</span></span>      | <span data-ttu-id="630cc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="630cc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="630cc-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="630cc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="630cc-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="630cc-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="630cc-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="630cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="630cc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="630cc-114">Not supported.</span></span>    |
|<span data-ttu-id="630cc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="630cc-115">Application</span></span> | <span data-ttu-id="630cc-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="630cc-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="630cc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="630cc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="630cc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="630cc-118">Optional query parameters</span></span>

<span data-ttu-id="630cc-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="630cc-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="630cc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="630cc-120">Request headers</span></span>
| <span data-ttu-id="630cc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="630cc-121">Name</span></span>           | <span data-ttu-id="630cc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="630cc-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="630cc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="630cc-123">Authorization</span></span>  | <span data-ttu-id="630cc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="630cc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="630cc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="630cc-126">Request body</span></span>

<span data-ttu-id="630cc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="630cc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="630cc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="630cc-128">Response</span></span>

<span data-ttu-id="630cc-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="630cc-129">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="630cc-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="630cc-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="630cc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="630cc-131">Request</span></span>
<span data-ttu-id="630cc-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="630cc-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="630cc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="630cc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/serviceprincipals
```
# <a name="c"></a>[<span data-ttu-id="630cc-134">C#</span><span class="sxs-lookup"><span data-stu-id="630cc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="630cc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="630cc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="630cc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="630cc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="630cc-137">Java</span><span class="sxs-lookup"><span data-stu-id="630cc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="630cc-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="630cc-138">Response</span></span>
<span data-ttu-id="630cc-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="630cc-139">Here is an example of the response.</span></span> 

> <span data-ttu-id="630cc-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="630cc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [{
        "id": "59e617e5-e447-4adc-8b88-00af644d7c92",
        "deletedDateTime": null,
        "accountEnabled": true,
        "appDisplayName": "My App",
        "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
        "appOwnerOrganizationId": "1bc1c026-2f7b-48a5-98da-afa2fd8bc7bc",
        "appRoleAssignmentRequired": false,
        "displayName": "foo",
        "homepage": null,
        "logoutUrl": null,
        "publisherName": "Contoso",
        "replyUrls": [],
        "servicePrincipalNames": [
        "f1bd758f-4a1a-4b71-aa20-a248a22a8928"
        ],
        "tags": [],
        "addIns": [],
        "appRoles": [],
        "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
        },
        "keyCredentials": [],
        "oauth2PermissionScopes": [],
        "passwordCredentials": []
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


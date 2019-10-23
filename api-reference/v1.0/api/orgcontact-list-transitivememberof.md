---
title: Listar transitiveMemberOf
description: Obter grupos dos quais o contato do organziational é membro. Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o usuário é um membro aninhado.
author: anchanda
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 97f787dad12e499b64d43714e3cbe7b27be36d39
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37633901"
---
# <a name="list-transitivememberof"></a><span data-ttu-id="d8d16-104">Listar transitiveMemberOf</span><span class="sxs-lookup"><span data-stu-id="d8d16-104">List transitiveMemberOf</span></span>

<span data-ttu-id="d8d16-105">Obter grupos dos quais esse [contato organizacional](../resources/orgcontact.md) é membro.</span><span class="sxs-lookup"><span data-stu-id="d8d16-105">Get groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="d8d16-106">A solicitação de API é transitiva e retorna todos os grupos dos quais o contato organizacional é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="d8d16-106">The API request is transitive, and returns all groups the organizational contact is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8d16-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8d16-107">Permissions</span></span>

<span data-ttu-id="d8d16-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8d16-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8d16-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8d16-110">Permission type</span></span>      | <span data-ttu-id="d8d16-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8d16-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8d16-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8d16-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d8d16-113">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="d8d16-113">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="d8d16-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8d16-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8d16-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8d16-115">Not supported.</span></span>    |
|<span data-ttu-id="d8d16-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8d16-116">Application</span></span> | <span data-ttu-id="d8d16-117">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="d8d16-117">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8d16-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8d16-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d8d16-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d8d16-119">Optional query parameters</span></span>

<span data-ttu-id="d8d16-120">Este método dá suporte a `$select` [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d8d16-120">This method supports the `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8d16-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8d16-121">Request headers</span></span>

| <span data-ttu-id="d8d16-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8d16-122">Header</span></span>       | <span data-ttu-id="d8d16-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d8d16-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d8d16-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8d16-124">Authorization</span></span>  | <span data-ttu-id="d8d16-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8d16-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d8d16-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8d16-127">Accept</span></span>  | <span data-ttu-id="d8d16-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d8d16-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8d16-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8d16-129">Request body</span></span>

<span data-ttu-id="d8d16-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8d16-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8d16-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8d16-131">Response</span></span>

<span data-ttu-id="d8d16-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8d16-132">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8d16-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8d16-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8d16-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8d16-134">Request</span></span>

<span data-ttu-id="d8d16-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8d16-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d8d16-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8d16-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_list_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/transitiveMemberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d8d16-137">C#</span><span class="sxs-lookup"><span data-stu-id="d8d16-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-list-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8d16-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8d16-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-list-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d8d16-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8d16-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-list-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d8d16-140">Java</span><span class="sxs-lookup"><span data-stu-id="d8d16-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-list-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d8d16-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8d16-141">Response</span></span>

<span data-ttu-id="d8d16-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d8d16-142">The following is an example of the response.</span></span>
><span data-ttu-id="d8d16-143">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d8d16-143">**Note**: The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List orgContact transitiveMemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

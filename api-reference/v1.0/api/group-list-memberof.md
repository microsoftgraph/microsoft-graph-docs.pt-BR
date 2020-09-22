---
title: Listar memberOf
description: 'Obtenha grupos dos quais um grupo é um membro direto. '
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a6a87d643c9cd0b53b4769f6943f4a6f8e779f5f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038617"
---
# <a name="list-memberof"></a><span data-ttu-id="80b7d-103">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="80b7d-103">List memberOf</span></span>

<span data-ttu-id="80b7d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80b7d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="80b7d-105">Obtenha grupos dos quais um grupo é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="80b7d-105">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="80b7d-p101">Essa operação não é transitiva. Ao contrário de obter Grupos do Microsoft 365 de um usuário, retorna todos os tipos de grupos, não apenas grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="80b7d-p101">This operation is not transitive. Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="80b7d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="80b7d-108">Permissions</span></span>
<span data-ttu-id="80b7d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80b7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80b7d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80b7d-111">Permission type</span></span>      | <span data-ttu-id="80b7d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80b7d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80b7d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80b7d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="80b7d-114">GroupMember.Read.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="80b7d-114">GroupMember.Read.All, Group.Read.All</span></span>    |
|<span data-ttu-id="80b7d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80b7d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80b7d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80b7d-116">Not supported.</span></span>    |
|<span data-ttu-id="80b7d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80b7d-117">Application</span></span> | <span data-ttu-id="80b7d-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="80b7d-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="80b7d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80b7d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80b7d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="80b7d-120">Optional query parameters</span></span>
<span data-ttu-id="80b7d-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="80b7d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80b7d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80b7d-122">Request headers</span></span>
| <span data-ttu-id="80b7d-123">Nome</span><span class="sxs-lookup"><span data-stu-id="80b7d-123">Name</span></span>       | <span data-ttu-id="80b7d-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="80b7d-124">Type</span></span> | <span data-ttu-id="80b7d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="80b7d-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="80b7d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="80b7d-126">Authorization</span></span>  | <span data-ttu-id="80b7d-127">string</span><span class="sxs-lookup"><span data-stu-id="80b7d-127">string</span></span>  | <span data-ttu-id="80b7d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80b7d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80b7d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80b7d-130">Request body</span></span>
<span data-ttu-id="80b7d-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="80b7d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80b7d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="80b7d-132">Response</span></span>
<span data-ttu-id="80b7d-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80b7d-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80b7d-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80b7d-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="80b7d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80b7d-135">Request</span></span>
<span data-ttu-id="80b7d-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="80b7d-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="80b7d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="80b7d-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="80b7d-138">C#</span><span class="sxs-lookup"><span data-stu-id="80b7d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80b7d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80b7d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80b7d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80b7d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80b7d-141">Java</span><span class="sxs-lookup"><span data-stu-id="80b7d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="80b7d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="80b7d-142">Response</span></span>
<span data-ttu-id="80b7d-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="80b7d-143">The following is an example of the response.</span></span>
><span data-ttu-id="80b7d-144">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="80b7d-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="80b7d-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80b7d-145">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


---
title: Listar memberOf
description: 'Obtenha grupos dos quais um grupo é um membro direto. '
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7f30b10ef9c6b33fc92b86b02fefe8c4c71c4a39
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125222"
---
# <a name="list-memberof"></a><span data-ttu-id="0e180-103">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="0e180-103">List memberOf</span></span>

<span data-ttu-id="0e180-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e180-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0e180-105">Obtenha grupos dos quais um grupo é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="0e180-105">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="0e180-p101">Essa operação não é transitiva. Ao contrário de obter Grupos do Office 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="0e180-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e180-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e180-108">Permissions</span></span>
<span data-ttu-id="0e180-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e180-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e180-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e180-111">Permission type</span></span>      | <span data-ttu-id="0e180-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e180-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e180-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e180-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0e180-114">GroupMember.Read.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e180-114">GroupMember.Read.All, Group.Read.All</span></span>    |
|<span data-ttu-id="0e180-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e180-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e180-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e180-116">Not supported.</span></span>    |
|<span data-ttu-id="0e180-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e180-117">Application</span></span> | <span data-ttu-id="0e180-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e180-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="0e180-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e180-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e180-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0e180-120">Optional query parameters</span></span>
<span data-ttu-id="0e180-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0e180-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e180-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e180-122">Request headers</span></span>
| <span data-ttu-id="0e180-123">Nome</span><span class="sxs-lookup"><span data-stu-id="0e180-123">Name</span></span>       | <span data-ttu-id="0e180-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e180-124">Type</span></span> | <span data-ttu-id="0e180-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e180-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0e180-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e180-126">Authorization</span></span>  | <span data-ttu-id="0e180-127">string</span><span class="sxs-lookup"><span data-stu-id="0e180-127">string</span></span>  | <span data-ttu-id="0e180-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e180-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e180-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e180-130">Request body</span></span>
<span data-ttu-id="0e180-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e180-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e180-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e180-132">Response</span></span>
<span data-ttu-id="0e180-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e180-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e180-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e180-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0e180-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e180-135">Request</span></span>
<span data-ttu-id="0e180-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e180-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0e180-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e180-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="0e180-138">C#</span><span class="sxs-lookup"><span data-stu-id="0e180-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e180-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e180-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e180-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e180-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e180-141">Java</span><span class="sxs-lookup"><span data-stu-id="0e180-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0e180-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e180-142">Response</span></span>
<span data-ttu-id="0e180-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0e180-143">The following is an example of the response.</span></span>
><span data-ttu-id="0e180-144">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0e180-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0e180-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e180-145">All the properties will be returned from an actual call.</span></span>
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

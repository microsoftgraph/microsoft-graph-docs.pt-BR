---
title: Listar proprietários
description: Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7ff45d17a039b1c1295dea1410acff7ed1c73612
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720540"
---
# <a name="list-owners"></a><span data-ttu-id="f53bc-104">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="f53bc-104">List owners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f53bc-p102">Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="f53bc-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f53bc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f53bc-107">Permissions</span></span>
<span data-ttu-id="f53bc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f53bc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f53bc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f53bc-110">Permission type</span></span>      | <span data-ttu-id="f53bc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f53bc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f53bc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f53bc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f53bc-113">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f53bc-113">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>    |
|<span data-ttu-id="f53bc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f53bc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f53bc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f53bc-115">Not supported.</span></span>    |
|<span data-ttu-id="f53bc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f53bc-116">Application</span></span> | <span data-ttu-id="f53bc-117">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f53bc-117">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f53bc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f53bc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f53bc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f53bc-119">Optional query parameters</span></span>
<span data-ttu-id="f53bc-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f53bc-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f53bc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f53bc-121">Request headers</span></span>
| <span data-ttu-id="f53bc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f53bc-122">Name</span></span>       | <span data-ttu-id="f53bc-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f53bc-123">Type</span></span> | <span data-ttu-id="f53bc-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f53bc-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f53bc-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f53bc-125">Authorization</span></span>  | <span data-ttu-id="f53bc-126">string</span><span class="sxs-lookup"><span data-stu-id="f53bc-126">string</span></span>  | <span data-ttu-id="f53bc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f53bc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f53bc-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f53bc-129">Request body</span></span>
<span data-ttu-id="f53bc-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f53bc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f53bc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f53bc-131">Response</span></span>
<span data-ttu-id="f53bc-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f53bc-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f53bc-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f53bc-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f53bc-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f53bc-134">Request</span></span>
<span data-ttu-id="f53bc-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f53bc-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f53bc-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f53bc-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/owners
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f53bc-137">C#</span><span class="sxs-lookup"><span data-stu-id="f53bc-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f53bc-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f53bc-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f53bc-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f53bc-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f53bc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f53bc-140">Response</span></span>
<span data-ttu-id="f53bc-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f53bc-141">The following is an example of the response.</span></span>
><span data-ttu-id="f53bc-142">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f53bc-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f53bc-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f53bc-143">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

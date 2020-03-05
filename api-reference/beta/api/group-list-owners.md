---
title: Listar proprietários
description: Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 98ab9bee1740d623dc962f7e0bf8df921e3ef407
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419419"
---
# <a name="list-owners"></a><span data-ttu-id="e86ab-104">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="e86ab-104">List owners</span></span>

<span data-ttu-id="e86ab-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e86ab-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e86ab-p102">Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="e86ab-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e86ab-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e86ab-108">Permissions</span></span>
<span data-ttu-id="e86ab-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e86ab-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e86ab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e86ab-111">Permission type</span></span>      | <span data-ttu-id="e86ab-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e86ab-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e86ab-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e86ab-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e86ab-114">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e86ab-114">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>    |
|<span data-ttu-id="e86ab-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e86ab-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e86ab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e86ab-116">Not supported.</span></span>    |
|<span data-ttu-id="e86ab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e86ab-117">Application</span></span> | <span data-ttu-id="e86ab-118">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e86ab-118">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e86ab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e86ab-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e86ab-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e86ab-120">Optional query parameters</span></span>
<span data-ttu-id="e86ab-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e86ab-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e86ab-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e86ab-122">Request headers</span></span>
| <span data-ttu-id="e86ab-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e86ab-123">Name</span></span>       | <span data-ttu-id="e86ab-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="e86ab-124">Type</span></span> | <span data-ttu-id="e86ab-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e86ab-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e86ab-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e86ab-126">Authorization</span></span>  | <span data-ttu-id="e86ab-127">string</span><span class="sxs-lookup"><span data-stu-id="e86ab-127">string</span></span>  | <span data-ttu-id="e86ab-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e86ab-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e86ab-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e86ab-130">Request body</span></span>
<span data-ttu-id="e86ab-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e86ab-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e86ab-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e86ab-132">Response</span></span>
<span data-ttu-id="e86ab-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e86ab-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e86ab-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e86ab-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e86ab-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e86ab-135">Request</span></span>
<span data-ttu-id="e86ab-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e86ab-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e86ab-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e86ab-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="e86ab-138">C#</span><span class="sxs-lookup"><span data-stu-id="e86ab-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e86ab-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e86ab-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e86ab-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e86ab-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e86ab-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e86ab-141">Response</span></span>
<span data-ttu-id="e86ab-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e86ab-142">The following is an example of the response.</span></span>
><span data-ttu-id="e86ab-143">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e86ab-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e86ab-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e86ab-144">All the properties will be returned from an actual call.</span></span>
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

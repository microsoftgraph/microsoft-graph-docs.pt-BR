---
title: Listar proprietários
description: 'Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo. '
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 57ca7bd1e84f507dbf59f515f6f7b2ec1ef020ed
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125215"
---
# <a name="list-owners"></a><span data-ttu-id="b90df-104">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="b90df-104">List owners</span></span>

<span data-ttu-id="b90df-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b90df-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b90df-p102">Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="b90df-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b90df-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b90df-108">Permissions</span></span>
<span data-ttu-id="b90df-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b90df-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b90df-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b90df-111">Permission type</span></span>      | <span data-ttu-id="b90df-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b90df-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b90df-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b90df-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b90df-114">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b90df-114">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="b90df-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b90df-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b90df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b90df-116">Not supported.</span></span>    |
|<span data-ttu-id="b90df-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b90df-117">Application</span></span> | <span data-ttu-id="b90df-118">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b90df-118">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="b90df-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b90df-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b90df-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b90df-120">Optional query parameters</span></span>
<span data-ttu-id="b90df-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b90df-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b90df-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b90df-122">Request headers</span></span>
| <span data-ttu-id="b90df-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b90df-123">Name</span></span>       | <span data-ttu-id="b90df-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b90df-124">Type</span></span> | <span data-ttu-id="b90df-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b90df-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b90df-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b90df-126">Authorization</span></span>  | <span data-ttu-id="b90df-127">string</span><span class="sxs-lookup"><span data-stu-id="b90df-127">string</span></span>  | <span data-ttu-id="b90df-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b90df-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b90df-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b90df-130">Request body</span></span>
<span data-ttu-id="b90df-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b90df-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b90df-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b90df-132">Response</span></span>
<span data-ttu-id="b90df-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b90df-133">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b90df-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b90df-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b90df-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b90df-135">Request</span></span>
<span data-ttu-id="b90df-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b90df-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b90df-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b90df-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="b90df-138">C#</span><span class="sxs-lookup"><span data-stu-id="b90df-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b90df-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b90df-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b90df-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b90df-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b90df-141">Java</span><span class="sxs-lookup"><span data-stu-id="b90df-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b90df-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b90df-142">Response</span></span>
<span data-ttu-id="b90df-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b90df-143">The following is an example of the response.</span></span>
><span data-ttu-id="b90df-144">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b90df-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b90df-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b90df-145">All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.user"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

---
title: Listar proprietários
description: 'Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo. '
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2294378620f6d02da7cb98be657fb587a8a7b46b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335408"
---
# <a name="list-owners"></a><span data-ttu-id="3a1cf-104">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="3a1cf-104">List owners</span></span>

<span data-ttu-id="3a1cf-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a1cf-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3a1cf-p102">Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores ou entidades de serviço que têm permissão para modificar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="3a1cf-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users or service principals who are allowed to modify the group object.</span></span> 

><span data-ttu-id="3a1cf-108">**Observação:** No momento, as entidades de serviço não estão listadas como proprietários de grupo devido à distribuição em estágios das entidades de serviço para o ponto de extremidade do Microsoft Graph v 1.0.</span><span class="sxs-lookup"><span data-stu-id="3a1cf-108">**Note:** Currently, service principals are not listed as group owners due to the staged rollout of service principals to the Microsoft Graph v1.0 endpoint.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a1cf-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a1cf-109">Permissions</span></span>
<span data-ttu-id="3a1cf-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a1cf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a1cf-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a1cf-112">Permission type</span></span>      | <span data-ttu-id="3a1cf-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a1cf-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a1cf-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a1cf-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3a1cf-115">Group. Read. All e User. ReadBasic. All, Group. Read. All e User. Read. All, Group. Read. All e User. ReadWrite. All, Group. Read. All e User. Read. All e Application. Read. All</span><span class="sxs-lookup"><span data-stu-id="3a1cf-115">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span>   |
|<span data-ttu-id="3a1cf-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a1cf-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a1cf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a1cf-117">Not supported.</span></span>    |
|<span data-ttu-id="3a1cf-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a1cf-118">Application</span></span> | <span data-ttu-id="3a1cf-119">Group. Read. All e User. Read. All, Group. Read. All e User. ReadWrite. All, Group. Read. All e User. Read. All e Application. Read. All</span><span class="sxs-lookup"><span data-stu-id="3a1cf-119">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="3a1cf-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a1cf-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a1cf-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3a1cf-121">Optional query parameters</span></span>
<span data-ttu-id="3a1cf-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3a1cf-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a1cf-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a1cf-123">Request headers</span></span>
| <span data-ttu-id="3a1cf-124">Nome</span><span class="sxs-lookup"><span data-stu-id="3a1cf-124">Name</span></span>       | <span data-ttu-id="3a1cf-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a1cf-125">Type</span></span> | <span data-ttu-id="3a1cf-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a1cf-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3a1cf-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a1cf-127">Authorization</span></span>  | <span data-ttu-id="3a1cf-128">string</span><span class="sxs-lookup"><span data-stu-id="3a1cf-128">string</span></span>  | <span data-ttu-id="3a1cf-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a1cf-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a1cf-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a1cf-131">Request body</span></span>
<span data-ttu-id="3a1cf-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a1cf-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a1cf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a1cf-133">Response</span></span>
<span data-ttu-id="3a1cf-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a1cf-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a1cf-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a1cf-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3a1cf-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a1cf-136">Request</span></span>
<span data-ttu-id="3a1cf-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a1cf-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3a1cf-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a1cf-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="3a1cf-139">C#</span><span class="sxs-lookup"><span data-stu-id="3a1cf-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a1cf-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a1cf-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a1cf-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a1cf-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a1cf-142">Java</span><span class="sxs-lookup"><span data-stu-id="3a1cf-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3a1cf-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a1cf-143">Response</span></span>
<span data-ttu-id="3a1cf-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3a1cf-144">The following is an example of the response.</span></span>
><span data-ttu-id="3a1cf-145">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3a1cf-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3a1cf-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a1cf-146">All the properties will be returned from an actual call.</span></span>
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

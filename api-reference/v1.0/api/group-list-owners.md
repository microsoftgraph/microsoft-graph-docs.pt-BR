---
title: Listar proprietários
description: 'Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo. '
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 767d1d399f7be629d3d4e71fd9412cab863e8c9f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063657"
---
# <a name="list-owners"></a><span data-ttu-id="2618f-104">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="2618f-104">List owners</span></span>

<span data-ttu-id="2618f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2618f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2618f-p102">Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="2618f-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users or service principals who are allowed to modify the group object.</span></span> 

><span data-ttu-id="2618f-108">**Observação:** No momento, as entidades de serviço não estão listadas como proprietários de grupo devido à distribuição em estágios das entidades de serviço para o ponto de extremidade do Microsoft Graph v 1.0.</span><span class="sxs-lookup"><span data-stu-id="2618f-108">**Note:** Currently, service principals are not listed as group owners due to the staged rollout of service principals to the Microsoft Graph v1.0 endpoint.</span></span>

## <a name="permissions"></a><span data-ttu-id="2618f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="2618f-109">Permissions</span></span>
<span data-ttu-id="2618f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2618f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2618f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2618f-112">Permission type</span></span>      | <span data-ttu-id="2618f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2618f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2618f-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2618f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2618f-115">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="2618f-115">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span>   |
|<span data-ttu-id="2618f-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2618f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2618f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2618f-117">Not supported.</span></span>    |
|<span data-ttu-id="2618f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2618f-118">Application</span></span> | <span data-ttu-id="2618f-119">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="2618f-119">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="2618f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2618f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2618f-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2618f-121">Optional query parameters</span></span>
<span data-ttu-id="2618f-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2618f-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2618f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2618f-123">Request headers</span></span>
| <span data-ttu-id="2618f-124">Nome</span><span class="sxs-lookup"><span data-stu-id="2618f-124">Name</span></span>       | <span data-ttu-id="2618f-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="2618f-125">Type</span></span> | <span data-ttu-id="2618f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="2618f-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2618f-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="2618f-127">Authorization</span></span>  | <span data-ttu-id="2618f-128">string</span><span class="sxs-lookup"><span data-stu-id="2618f-128">string</span></span>  | <span data-ttu-id="2618f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2618f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2618f-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2618f-131">Request body</span></span>
<span data-ttu-id="2618f-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2618f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2618f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2618f-133">Response</span></span>
<span data-ttu-id="2618f-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2618f-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2618f-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2618f-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2618f-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2618f-136">Request</span></span>
<span data-ttu-id="2618f-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2618f-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2618f-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="2618f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="2618f-139">C#</span><span class="sxs-lookup"><span data-stu-id="2618f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2618f-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2618f-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2618f-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2618f-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2618f-142">Java</span><span class="sxs-lookup"><span data-stu-id="2618f-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2618f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="2618f-143">Response</span></span>
<span data-ttu-id="2618f-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2618f-144">The following is an example of the response.</span></span>
><span data-ttu-id="2618f-145">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2618f-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2618f-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2618f-146">All the properties will be returned from an actual call.</span></span>
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


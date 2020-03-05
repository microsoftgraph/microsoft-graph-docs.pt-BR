---
title: Grupo de lista memberOf
description: Obter grupos e unidades administrativas dos quais o grupo é membro direto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4b4edb12a1b620c77f844d1e2a5d5f5a7751a249
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419433"
---
# <a name="list-group-memberof"></a><span data-ttu-id="48156-103">Grupo de lista memberOf</span><span class="sxs-lookup"><span data-stu-id="48156-103">List group memberOf</span></span>

<span data-ttu-id="48156-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="48156-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48156-105">Obter grupos e unidades administrativas dos quais o grupo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="48156-105">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="48156-106">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="48156-106">This operation is not transitive.</span></span> <span data-ttu-id="48156-107">Ao contrário de obter os grupos do Office 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="48156-107">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="48156-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="48156-108">Permissions</span></span>

<span data-ttu-id="48156-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48156-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48156-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48156-111">Permission type</span></span>      | <span data-ttu-id="48156-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48156-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48156-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48156-113">Delegated (work or school account)</span></span> | <span data-ttu-id="48156-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48156-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="48156-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48156-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48156-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48156-116">Not supported.</span></span>    |
|<span data-ttu-id="48156-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48156-117">Application</span></span> | <span data-ttu-id="48156-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48156-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="48156-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48156-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48156-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="48156-120">Optional query parameters</span></span>
<span data-ttu-id="48156-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="48156-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48156-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48156-122">Request headers</span></span>
| <span data-ttu-id="48156-123">Nome</span><span class="sxs-lookup"><span data-stu-id="48156-123">Name</span></span>       | <span data-ttu-id="48156-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="48156-124">Type</span></span> | <span data-ttu-id="48156-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="48156-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="48156-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="48156-126">Authorization</span></span>  | <span data-ttu-id="48156-127">string</span><span class="sxs-lookup"><span data-stu-id="48156-127">string</span></span>  | <span data-ttu-id="48156-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48156-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48156-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48156-130">Request body</span></span>
<span data-ttu-id="48156-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="48156-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48156-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="48156-132">Response</span></span>
<span data-ttu-id="48156-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48156-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48156-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48156-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="48156-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48156-135">Request</span></span>

<span data-ttu-id="48156-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="48156-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="48156-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="48156-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="48156-138">C#</span><span class="sxs-lookup"><span data-stu-id="48156-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48156-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48156-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48156-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48156-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="48156-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="48156-141">Response</span></span>

<span data-ttu-id="48156-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="48156-142">The following is an example of the response.</span></span>
><span data-ttu-id="48156-143">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="48156-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="48156-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48156-144">All the properties will be returned from an actual call.</span></span>
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

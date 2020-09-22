---
title: Listar membros
description: Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos organizacionais, dispositivos, entidades de serviço e outros grupos como membros.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6eebc7a1f9a33b1cebf5d935b4ff5af0a4b3a790
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057630"
---
# <a name="list-members"></a><span data-ttu-id="a9d92-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="a9d92-104">List members</span></span>

<span data-ttu-id="a9d92-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9d92-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a9d92-106">Obtenha uma lista dos membros diretos do grupo.</span><span class="sxs-lookup"><span data-stu-id="a9d92-106">Get a list of the group's direct members.</span></span> <span data-ttu-id="a9d92-107">Um grupo pode ter usuários, contatos organizacionais, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="a9d92-107">A group can have users, organizational contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="a9d92-108">No momento, as entidades de serviço não estão listadas como membros de grupo devido à distribuição em estágios das entidades de serviço para o ponto de extremidade do Graph v 1.0.</span><span class="sxs-lookup"><span data-stu-id="a9d92-108">Currently service principals are not listed as group members due to staged roll-out of service principals on Graph V1.0 endpoint.</span></span> <span data-ttu-id="a9d92-109">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="a9d92-109">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9d92-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9d92-110">Permissions</span></span>
<span data-ttu-id="a9d92-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9d92-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9d92-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9d92-113">Permission type</span></span>      | <span data-ttu-id="a9d92-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9d92-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9d92-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9d92-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a9d92-116">User.ReadBasic.All, User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9d92-116">User.ReadBasic.All, User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="a9d92-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9d92-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9d92-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9d92-118">Not supported.</span></span>    |
|<span data-ttu-id="a9d92-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9d92-119">Application</span></span> | <span data-ttu-id="a9d92-120">User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9d92-120">User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a9d92-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9d92-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9d92-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a9d92-122">Optional query parameters</span></span>
<span data-ttu-id="a9d92-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a9d92-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9d92-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9d92-124">Request headers</span></span>
| <span data-ttu-id="a9d92-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9d92-125">Header</span></span>       | <span data-ttu-id="a9d92-126">Valor</span><span class="sxs-lookup"><span data-stu-id="a9d92-126">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="a9d92-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9d92-127">Authorization</span></span>  | <span data-ttu-id="a9d92-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9d92-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9d92-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9d92-130">Request body</span></span>
<span data-ttu-id="a9d92-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9d92-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9d92-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9d92-132">Response</span></span>
<span data-ttu-id="a9d92-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9d92-133">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9d92-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9d92-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a9d92-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9d92-135">Request</span></span>
<span data-ttu-id="a9d92-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9d92-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9d92-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9d92-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="a9d92-138">C#</span><span class="sxs-lookup"><span data-stu-id="a9d92-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9d92-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9d92-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9d92-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9d92-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9d92-141">Java</span><span class="sxs-lookup"><span data-stu-id="a9d92-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a9d92-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9d92-142">Response</span></span>
<span data-ttu-id="a9d92-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9d92-143">The following is an example of the response.</span></span>
><span data-ttu-id="a9d92-144">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a9d92-144">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


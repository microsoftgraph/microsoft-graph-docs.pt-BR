---
title: Listar membros
description: Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos organizacionais e outros grupos como membros.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: fdb70c70f066c459b2188e90fce40ed73adc0050
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181712"
---
# <a name="list-members"></a><span data-ttu-id="6627b-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="6627b-104">List members</span></span>

<span data-ttu-id="6627b-p102">Namespace: microsoft.graph Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos organizacionais e outros grupos como membros. Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="6627b-p102">Namespace: microsoft.graph Get a list of the group's direct members. A group can have users, organizational contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="6627b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6627b-108">Permissions</span></span>
<span data-ttu-id="6627b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6627b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6627b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6627b-111">Permission type</span></span>      | <span data-ttu-id="6627b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6627b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6627b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6627b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6627b-114">User.ReadBasic.All, User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6627b-114">User.ReadBasic.All, User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="6627b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6627b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6627b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6627b-116">Not supported.</span></span>    |
|<span data-ttu-id="6627b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6627b-117">Application</span></span> | <span data-ttu-id="6627b-118">User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6627b-118">User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="6627b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6627b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6627b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6627b-120">Optional query parameters</span></span>
<span data-ttu-id="6627b-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6627b-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6627b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6627b-122">Request headers</span></span>
| <span data-ttu-id="6627b-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6627b-123">Header</span></span>       | <span data-ttu-id="6627b-124">Valor</span><span class="sxs-lookup"><span data-stu-id="6627b-124">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="6627b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6627b-125">Authorization</span></span>  | <span data-ttu-id="6627b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6627b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6627b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6627b-128">Request body</span></span>
<span data-ttu-id="6627b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6627b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6627b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6627b-130">Response</span></span>
<span data-ttu-id="6627b-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6627b-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6627b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6627b-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6627b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6627b-133">Request</span></span>
<span data-ttu-id="6627b-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6627b-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6627b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6627b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="6627b-136">C#</span><span class="sxs-lookup"><span data-stu-id="6627b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6627b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6627b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6627b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6627b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6627b-139">Java</span><span class="sxs-lookup"><span data-stu-id="6627b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6627b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6627b-140">Response</span></span>
<span data-ttu-id="6627b-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6627b-141">The following is an example of the response.</span></span>
><span data-ttu-id="6627b-142">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6627b-142">**Note:** The response object shown here might be shortened for readability.</span></span> 
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

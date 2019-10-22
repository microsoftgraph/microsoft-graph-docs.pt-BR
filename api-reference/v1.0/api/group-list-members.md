---
title: Listar membros
description: Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos organizacionais e outros grupos como membros.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a3a2dd63e5f91ce9df26d6b649d3d005bf73f545
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37622558"
---
# <a name="list-members"></a><span data-ttu-id="18d34-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="18d34-104">List members</span></span>
<span data-ttu-id="18d34-p102">Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos organizacionais e outros grupos como membros. Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="18d34-p102">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="18d34-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="18d34-108">Permissions</span></span>
<span data-ttu-id="18d34-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18d34-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18d34-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18d34-111">Permission type</span></span>      | <span data-ttu-id="18d34-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18d34-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18d34-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18d34-113">Delegated (work or school account)</span></span> | <span data-ttu-id="18d34-114">User. ReadBasic. All, User. Read. All, Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="18d34-114">User.ReadBasic.All, User.Read.All, Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="18d34-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18d34-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18d34-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18d34-116">Not supported.</span></span>    |
|<span data-ttu-id="18d34-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18d34-117">Application</span></span> | <span data-ttu-id="18d34-118">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="18d34-118">User.Read.All, Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18d34-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18d34-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18d34-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="18d34-120">Optional query parameters</span></span>
<span data-ttu-id="18d34-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="18d34-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18d34-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18d34-122">Request headers</span></span>
| <span data-ttu-id="18d34-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18d34-123">Header</span></span>       | <span data-ttu-id="18d34-124">Valor</span><span class="sxs-lookup"><span data-stu-id="18d34-124">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="18d34-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="18d34-125">Authorization</span></span>  | <span data-ttu-id="18d34-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18d34-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18d34-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18d34-128">Request body</span></span>
<span data-ttu-id="18d34-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="18d34-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18d34-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="18d34-130">Response</span></span>
<span data-ttu-id="18d34-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18d34-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18d34-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18d34-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="18d34-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18d34-133">Request</span></span>
<span data-ttu-id="18d34-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="18d34-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="18d34-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="18d34-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="18d34-136">C#</span><span class="sxs-lookup"><span data-stu-id="18d34-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18d34-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18d34-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="18d34-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18d34-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="18d34-139">Java</span><span class="sxs-lookup"><span data-stu-id="18d34-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="18d34-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="18d34-140">Response</span></span>
<span data-ttu-id="18d34-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="18d34-141">The following is an example of the response.</span></span>
><span data-ttu-id="18d34-142">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="18d34-142">**Note:** The response object shown here might be shortened for readability.</span></span> 
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

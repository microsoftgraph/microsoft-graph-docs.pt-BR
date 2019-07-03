---
title: Listar membros
description: Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos e outros grupos como membros.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: f03e1b62d4e1e765cd552802af22361a4e88419a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441636"
---
# <a name="list-members"></a><span data-ttu-id="f16ac-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="f16ac-104">List members</span></span>
<span data-ttu-id="f16ac-p102">Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos e outros grupos como membros. Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="f16ac-p102">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="f16ac-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f16ac-108">Permissions</span></span>
<span data-ttu-id="f16ac-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f16ac-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f16ac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f16ac-111">Permission type</span></span>      | <span data-ttu-id="f16ac-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f16ac-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f16ac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f16ac-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f16ac-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f16ac-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="f16ac-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f16ac-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f16ac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f16ac-116">Not supported.</span></span>    |
|<span data-ttu-id="f16ac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f16ac-117">Application</span></span> | <span data-ttu-id="f16ac-118">User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f16ac-118">User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f16ac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f16ac-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f16ac-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f16ac-120">Optional query parameters</span></span>
<span data-ttu-id="f16ac-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f16ac-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f16ac-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f16ac-122">Request headers</span></span>
| <span data-ttu-id="f16ac-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f16ac-123">Name</span></span>       | <span data-ttu-id="f16ac-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f16ac-124">Type</span></span> | <span data-ttu-id="f16ac-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f16ac-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f16ac-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="f16ac-126">Authorization</span></span>  | <span data-ttu-id="f16ac-127">string</span><span class="sxs-lookup"><span data-stu-id="f16ac-127">string</span></span>  | <span data-ttu-id="f16ac-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f16ac-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f16ac-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f16ac-130">Request body</span></span>
<span data-ttu-id="f16ac-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f16ac-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f16ac-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f16ac-132">Response</span></span>
<span data-ttu-id="f16ac-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f16ac-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f16ac-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f16ac-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f16ac-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f16ac-135">Request</span></span>
<span data-ttu-id="f16ac-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f16ac-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f16ac-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f16ac-137">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f16ac-138">C#</span><span class="sxs-lookup"><span data-stu-id="f16ac-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f16ac-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="f16ac-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f16ac-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f16ac-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f16ac-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f16ac-141">Response</span></span>
<span data-ttu-id="f16ac-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f16ac-142">The following is an example of the response.</span></span>
><span data-ttu-id="f16ac-143">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f16ac-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f16ac-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f16ac-144">All the properties will be returned from an actual call.</span></span>
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

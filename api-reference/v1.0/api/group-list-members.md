---
title: Listar membros
description: Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos e outros grupos como membros.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 6c79b4bd4ee3059e693e63817420e1c5d0b8d612
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279321"
---
# <a name="list-members"></a><span data-ttu-id="698cd-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="698cd-104">List members</span></span>
<span data-ttu-id="698cd-p102">Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos e outros grupos como membros. Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="698cd-p102">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="698cd-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="698cd-108">Permissions</span></span>
<span data-ttu-id="698cd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="698cd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="698cd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="698cd-111">Permission type</span></span>      | <span data-ttu-id="698cd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="698cd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="698cd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="698cd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="698cd-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="698cd-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="698cd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="698cd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="698cd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="698cd-116">Not supported.</span></span>    |
|<span data-ttu-id="698cd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="698cd-117">Application</span></span> | <span data-ttu-id="698cd-118">User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="698cd-118">User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="698cd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="698cd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="698cd-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="698cd-120">Optional query parameters</span></span>
<span data-ttu-id="698cd-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="698cd-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="698cd-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="698cd-122">Request headers</span></span>
| <span data-ttu-id="698cd-123">Nome</span><span class="sxs-lookup"><span data-stu-id="698cd-123">Name</span></span>       | <span data-ttu-id="698cd-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="698cd-124">Type</span></span> | <span data-ttu-id="698cd-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="698cd-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="698cd-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="698cd-126">Authorization</span></span>  | <span data-ttu-id="698cd-127">string</span><span class="sxs-lookup"><span data-stu-id="698cd-127">string</span></span>  | <span data-ttu-id="698cd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="698cd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="698cd-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="698cd-130">Request body</span></span>
<span data-ttu-id="698cd-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="698cd-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="698cd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="698cd-132">Response</span></span>
<span data-ttu-id="698cd-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="698cd-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="698cd-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="698cd-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="698cd-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="698cd-135">Request</span></span>
<span data-ttu-id="698cd-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="698cd-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```

#### <a name="response"></a><span data-ttu-id="698cd-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="698cd-137">Response</span></span>
<span data-ttu-id="698cd-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="698cd-138">The following is an example of the response.</span></span>
><span data-ttu-id="698cd-139">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="698cd-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="698cd-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="698cd-140">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="698cd-141">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="698cd-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="698cd-142">C#</span><span class="sxs-lookup"><span data-stu-id="698cd-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_members-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="698cd-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="698cd-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_members-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="698cd-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="698cd-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_members-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-list-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

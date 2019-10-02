---
title: Membros do grupo de lista
description: Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros. Essa operação não é transitiva.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e2191102e62cacadddcbbbb270b6afe16af93ff9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356230"
---
# <a name="list-group-members"></a><span data-ttu-id="b8889-105">Membros do grupo de lista</span><span class="sxs-lookup"><span data-stu-id="b8889-105">List group members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8889-106">Obtenha uma lista dos membros diretos do grupo.</span><span class="sxs-lookup"><span data-stu-id="b8889-106">Get a list of the group's direct members.</span></span> <span data-ttu-id="b8889-107">Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="b8889-107">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="b8889-108">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="b8889-108">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8889-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8889-109">Permissions</span></span>

<span data-ttu-id="b8889-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8889-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8889-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8889-112">Permission type</span></span>      | <span data-ttu-id="b8889-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8889-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8889-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8889-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b8889-115">User. ReadBasic. All, User. Read. All, Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="b8889-115">User.ReadBasic.All, User.Read.All, Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="b8889-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8889-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8889-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8889-117">Not supported.</span></span>    |
|<span data-ttu-id="b8889-118">Application</span><span class="sxs-lookup"><span data-stu-id="b8889-118">Application</span></span> | <span data-ttu-id="b8889-119">Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8889-119">Group.Read.All, Directory.Read.All</span></span> |

> <span data-ttu-id="b8889-120">Observação: para listar os membros de um grupo de associação oculto, a permissão member. Read. Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="b8889-120">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>
 
## <a name="http-request"></a><span data-ttu-id="b8889-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8889-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8889-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b8889-122">Optional query parameters</span></span>
<span data-ttu-id="b8889-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8889-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8889-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8889-124">Request headers</span></span>
| <span data-ttu-id="b8889-125">Nome</span><span class="sxs-lookup"><span data-stu-id="b8889-125">Name</span></span>       | <span data-ttu-id="b8889-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8889-126">Type</span></span> | <span data-ttu-id="b8889-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8889-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b8889-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8889-128">Authorization</span></span>  | <span data-ttu-id="b8889-129">string</span><span class="sxs-lookup"><span data-stu-id="b8889-129">string</span></span>  | <span data-ttu-id="b8889-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8889-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8889-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8889-132">Request body</span></span>
<span data-ttu-id="b8889-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8889-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8889-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8889-134">Response</span></span>
<span data-ttu-id="b8889-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8889-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8889-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8889-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b8889-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8889-137">Request</span></span>
<span data-ttu-id="b8889-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8889-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b8889-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8889-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b8889-140">C#</span><span class="sxs-lookup"><span data-stu-id="b8889-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8889-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8889-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b8889-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8889-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b8889-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8889-143">Response</span></span>
<span data-ttu-id="b8889-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8889-144">The following is an example of the response.</span></span>
><span data-ttu-id="b8889-145">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b8889-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b8889-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8889-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
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
  "description": "List group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

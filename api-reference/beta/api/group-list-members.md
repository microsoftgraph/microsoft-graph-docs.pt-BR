---
title: Membros do grupo de lista
description: Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros. Essa operação não é transitiva.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 25f2585647e81afdf4abb9a2257b9548f1847c37
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419423"
---
# <a name="list-group-members"></a><span data-ttu-id="ceaa8-105">Membros do grupo de lista</span><span class="sxs-lookup"><span data-stu-id="ceaa8-105">List group members</span></span>

<span data-ttu-id="ceaa8-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ceaa8-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ceaa8-107">Obtenha uma lista dos membros diretos do grupo.</span><span class="sxs-lookup"><span data-stu-id="ceaa8-107">Get a list of the group's direct members.</span></span> <span data-ttu-id="ceaa8-108">Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="ceaa8-108">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="ceaa8-109">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="ceaa8-109">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ceaa8-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="ceaa8-110">Permissions</span></span>

<span data-ttu-id="ceaa8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ceaa8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ceaa8-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ceaa8-113">Permission type</span></span>      | <span data-ttu-id="ceaa8-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ceaa8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ceaa8-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ceaa8-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ceaa8-116">User. ReadBasic. All, User. Read. All, Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="ceaa8-116">User.ReadBasic.All, User.Read.All, Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="ceaa8-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ceaa8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ceaa8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ceaa8-118">Not supported.</span></span>    |
|<span data-ttu-id="ceaa8-119">Application</span><span class="sxs-lookup"><span data-stu-id="ceaa8-119">Application</span></span> | <span data-ttu-id="ceaa8-120">Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ceaa8-120">Group.Read.All, Directory.Read.All</span></span> |

> <span data-ttu-id="ceaa8-121">Observação: para listar os membros de um grupo de associação oculto, a permissão member. Read. Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="ceaa8-121">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]
 
## <a name="http-request"></a><span data-ttu-id="ceaa8-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ceaa8-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ceaa8-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ceaa8-123">Optional query parameters</span></span>
<span data-ttu-id="ceaa8-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ceaa8-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ceaa8-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ceaa8-125">Request headers</span></span>
| <span data-ttu-id="ceaa8-126">Nome</span><span class="sxs-lookup"><span data-stu-id="ceaa8-126">Name</span></span>       | <span data-ttu-id="ceaa8-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="ceaa8-127">Type</span></span> | <span data-ttu-id="ceaa8-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ceaa8-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ceaa8-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="ceaa8-129">Authorization</span></span>  | <span data-ttu-id="ceaa8-130">string</span><span class="sxs-lookup"><span data-stu-id="ceaa8-130">string</span></span>  | <span data-ttu-id="ceaa8-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ceaa8-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ceaa8-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ceaa8-133">Request body</span></span>
<span data-ttu-id="ceaa8-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ceaa8-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ceaa8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceaa8-135">Response</span></span>
<span data-ttu-id="ceaa8-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ceaa8-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceaa8-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ceaa8-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ceaa8-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ceaa8-138">Request</span></span>
<span data-ttu-id="ceaa8-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ceaa8-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ceaa8-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ceaa8-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="ceaa8-141">C#</span><span class="sxs-lookup"><span data-stu-id="ceaa8-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ceaa8-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ceaa8-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ceaa8-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ceaa8-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ceaa8-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceaa8-144">Response</span></span>
<span data-ttu-id="ceaa8-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ceaa8-145">The following is an example of the response.</span></span>
><span data-ttu-id="ceaa8-146">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ceaa8-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ceaa8-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ceaa8-147">All the properties will be returned from an actual call.</span></span>
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

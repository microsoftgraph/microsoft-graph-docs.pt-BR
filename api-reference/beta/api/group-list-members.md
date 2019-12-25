---
title: Membros do grupo de lista
description: Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros. Essa operação não é transitiva.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4d74380ab35e90002af2919b67b63b4a50fb7dcd
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869624"
---
# <a name="list-group-members"></a><span data-ttu-id="41b84-105">Membros do grupo de lista</span><span class="sxs-lookup"><span data-stu-id="41b84-105">List group members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41b84-106">Obtenha uma lista dos membros diretos do grupo.</span><span class="sxs-lookup"><span data-stu-id="41b84-106">Get a list of the group's direct members.</span></span> <span data-ttu-id="41b84-107">Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="41b84-107">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="41b84-108">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="41b84-108">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="41b84-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="41b84-109">Permissions</span></span>

<span data-ttu-id="41b84-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41b84-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41b84-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41b84-112">Permission type</span></span>      | <span data-ttu-id="41b84-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41b84-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41b84-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41b84-114">Delegated (work or school account)</span></span> | <span data-ttu-id="41b84-115">User. ReadBasic. All, User. Read. All, Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="41b84-115">User.ReadBasic.All, User.Read.All, Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="41b84-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41b84-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41b84-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41b84-117">Not supported.</span></span>    |
|<span data-ttu-id="41b84-118">Application</span><span class="sxs-lookup"><span data-stu-id="41b84-118">Application</span></span> | <span data-ttu-id="41b84-119">Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="41b84-119">Group.Read.All, Directory.Read.All</span></span> |

> <span data-ttu-id="41b84-120">Observação: para listar os membros de um grupo de associação oculto, a permissão member. Read. Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="41b84-120">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]
 
## <a name="http-request"></a><span data-ttu-id="41b84-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41b84-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41b84-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="41b84-122">Optional query parameters</span></span>
<span data-ttu-id="41b84-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="41b84-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41b84-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41b84-124">Request headers</span></span>
| <span data-ttu-id="41b84-125">Nome</span><span class="sxs-lookup"><span data-stu-id="41b84-125">Name</span></span>       | <span data-ttu-id="41b84-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="41b84-126">Type</span></span> | <span data-ttu-id="41b84-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="41b84-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="41b84-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="41b84-128">Authorization</span></span>  | <span data-ttu-id="41b84-129">string</span><span class="sxs-lookup"><span data-stu-id="41b84-129">string</span></span>  | <span data-ttu-id="41b84-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41b84-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41b84-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41b84-132">Request body</span></span>
<span data-ttu-id="41b84-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41b84-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41b84-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="41b84-134">Response</span></span>
<span data-ttu-id="41b84-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41b84-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41b84-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41b84-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="41b84-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41b84-137">Request</span></span>
<span data-ttu-id="41b84-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="41b84-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="41b84-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="41b84-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="41b84-140">C#</span><span class="sxs-lookup"><span data-stu-id="41b84-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41b84-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41b84-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="41b84-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41b84-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="41b84-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="41b84-143">Response</span></span>
<span data-ttu-id="41b84-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41b84-144">The following is an example of the response.</span></span>
><span data-ttu-id="41b84-145">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="41b84-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="41b84-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41b84-146">All the properties will be returned from an actual call.</span></span>
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

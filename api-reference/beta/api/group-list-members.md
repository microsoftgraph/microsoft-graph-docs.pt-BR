---
title: Membros do grupo de lista
description: Obtenha uma lista dos membros diretos do grupo.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: feae4be3a16254e15548f53bb19d55d186fa1ac4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43396945"
---
# <a name="list-group-members"></a><span data-ttu-id="5aebf-103">Membros do grupo de lista</span><span class="sxs-lookup"><span data-stu-id="5aebf-103">List group members</span></span>

<span data-ttu-id="5aebf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aebf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5aebf-105">Obtenha uma lista dos membros diretos do grupo.</span><span class="sxs-lookup"><span data-stu-id="5aebf-105">Get a list of the group's direct members.</span></span> <span data-ttu-id="5aebf-106">Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="5aebf-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="5aebf-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="5aebf-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="5aebf-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5aebf-108">Permissions</span></span>

<span data-ttu-id="5aebf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5aebf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5aebf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5aebf-111">Permission type</span></span>      | <span data-ttu-id="5aebf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5aebf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5aebf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5aebf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5aebf-114">User. ReadBasic. All, User. Read. All, Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="5aebf-114">User.ReadBasic.All, User.Read.All, Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="5aebf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5aebf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5aebf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5aebf-116">Not supported.</span></span>    |
|<span data-ttu-id="5aebf-117">Application</span><span class="sxs-lookup"><span data-stu-id="5aebf-117">Application</span></span> | <span data-ttu-id="5aebf-118">Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5aebf-118">Group.Read.All, Directory.Read.All</span></span> |

> <span data-ttu-id="5aebf-119">Observação: para listar os membros de um grupo de associação oculto, a permissão member. Read. Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="5aebf-119">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]
 
## <a name="http-request"></a><span data-ttu-id="5aebf-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5aebf-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5aebf-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5aebf-121">Optional query parameters</span></span>
<span data-ttu-id="5aebf-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5aebf-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5aebf-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5aebf-123">Request headers</span></span>
| <span data-ttu-id="5aebf-124">Nome</span><span class="sxs-lookup"><span data-stu-id="5aebf-124">Name</span></span>       | <span data-ttu-id="5aebf-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="5aebf-125">Type</span></span> | <span data-ttu-id="5aebf-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="5aebf-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5aebf-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="5aebf-127">Authorization</span></span>  | <span data-ttu-id="5aebf-128">string</span><span class="sxs-lookup"><span data-stu-id="5aebf-128">string</span></span>  | <span data-ttu-id="5aebf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5aebf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5aebf-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5aebf-131">Request body</span></span>
<span data-ttu-id="5aebf-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5aebf-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5aebf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aebf-133">Response</span></span>
<span data-ttu-id="5aebf-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5aebf-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5aebf-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5aebf-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5aebf-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5aebf-136">Request</span></span>
<span data-ttu-id="5aebf-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5aebf-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5aebf-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="5aebf-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="5aebf-139">C#</span><span class="sxs-lookup"><span data-stu-id="5aebf-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5aebf-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5aebf-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5aebf-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5aebf-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5aebf-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aebf-142">Response</span></span>
<span data-ttu-id="5aebf-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5aebf-143">The following is an example of the response.</span></span>
><span data-ttu-id="5aebf-144">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5aebf-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5aebf-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5aebf-145">All the properties will be returned from an actual call.</span></span>
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

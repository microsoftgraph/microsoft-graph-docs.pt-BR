---
title: Membros transitivos do grupo de lista
description: Obtenha uma lista dos membros do grupo. Um grupo pode ter usuários, dispositivos, contatos organizacionais e outros grupos como membros. Essa operação é transitiva e retorna uma lista simples de todos os membros aninhados.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 99a4abafb5cb879f2f8b7f721a237495055bcde7
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125131"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="3551e-105">Membros transitivos do grupo de lista</span><span class="sxs-lookup"><span data-stu-id="3551e-105">List group transitive members</span></span>

<span data-ttu-id="3551e-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3551e-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3551e-107">Obtenha uma lista dos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="3551e-107">Get a list of the group's members.</span></span> <span data-ttu-id="3551e-108">Um grupo pode ter usuários, dispositivos, contatos organizacionais e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="3551e-108">A group can have users, devices, organizational contacts, and other groups as members.</span></span> <span data-ttu-id="3551e-109">Essa operação é transitiva e retorna uma lista simples de todos os membros aninhados.</span><span class="sxs-lookup"><span data-stu-id="3551e-109">This operation is transitive and returns a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="3551e-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="3551e-110">Permissions</span></span>

<span data-ttu-id="3551e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3551e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3551e-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3551e-113">Permission type</span></span>      | <span data-ttu-id="3551e-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3551e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3551e-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3551e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3551e-116">Directory. Read. All, Directory. AccessAsUser. All, User. ReadBasic. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="3551e-116">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="3551e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3551e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3551e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3551e-118">Not supported.</span></span>    |
|<span data-ttu-id="3551e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3551e-119">Application</span></span> | <span data-ttu-id="3551e-120">Directory. Read. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="3551e-120">Directory.Read.All, User.Read.All</span></span> |

><span data-ttu-id="3551e-121">**Observação:** Para listar os membros de um grupo de associação oculto, a permissão member. Read. Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="3551e-121">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="3551e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3551e-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3551e-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3551e-123">Optional query parameters</span></span>

<span data-ttu-id="3551e-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3551e-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3551e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3551e-125">Request headers</span></span>

| <span data-ttu-id="3551e-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3551e-126">Header</span></span>       | <span data-ttu-id="3551e-127">Valor</span><span class="sxs-lookup"><span data-stu-id="3551e-127">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="3551e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="3551e-128">Authorization</span></span>  | <span data-ttu-id="3551e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3551e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3551e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3551e-131">Request body</span></span>

<span data-ttu-id="3551e-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3551e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3551e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3551e-133">Response</span></span>

<span data-ttu-id="3551e-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3551e-134">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3551e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3551e-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="3551e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3551e-136">Request</span></span>

<span data-ttu-id="3551e-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3551e-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3551e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3551e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="3551e-139">C#</span><span class="sxs-lookup"><span data-stu-id="3551e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3551e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3551e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3551e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3551e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3551e-142">Java</span><span class="sxs-lookup"><span data-stu-id="3551e-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3551e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3551e-143">Response</span></span>

<span data-ttu-id="3551e-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3551e-144">The following is an example of the response.</span></span>
><span data-ttu-id="3551e-145">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3551e-145">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

---
title: Membros transitivos do grupo de lista
description: Obtenha uma lista dos membros do grupo. Um grupo pode ter usuários, dispositivos, contatos organizacionais e outros grupos como membros. Essa operação é transitiva e retorna uma lista simples de todos os membros aninhados.
author: anchanda
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: cf4087675804b3bd873699634c527db9038ffe8e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869882"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="43c52-105">Membros transitivos do grupo de lista</span><span class="sxs-lookup"><span data-stu-id="43c52-105">List group transitive members</span></span>

<span data-ttu-id="43c52-106">Obtenha uma lista dos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="43c52-106">Get a list of the group's members.</span></span> <span data-ttu-id="43c52-107">Um grupo pode ter usuários, dispositivos, contatos organizacionais e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="43c52-107">A group can have users, devices, organizational contacts, and other groups as members.</span></span> <span data-ttu-id="43c52-108">Essa operação é transitiva e retorna uma lista simples de todos os membros aninhados.</span><span class="sxs-lookup"><span data-stu-id="43c52-108">This operation is transitive and returns a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="43c52-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="43c52-109">Permissions</span></span>

<span data-ttu-id="43c52-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43c52-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43c52-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43c52-112">Permission type</span></span>      | <span data-ttu-id="43c52-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43c52-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43c52-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43c52-114">Delegated (work or school account)</span></span> | <span data-ttu-id="43c52-115">Directory. Read. All, Directory. AccessAsUser. All, User. ReadBasic. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="43c52-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="43c52-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43c52-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43c52-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43c52-117">Not supported.</span></span>    |
|<span data-ttu-id="43c52-118">Application</span><span class="sxs-lookup"><span data-stu-id="43c52-118">Application</span></span> | <span data-ttu-id="43c52-119">Directory. Read. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="43c52-119">Directory.Read.All, User.Read.All</span></span> |

><span data-ttu-id="43c52-120">**Observação:** Para listar os membros de um grupo de associação oculto, a permissão member. Read. Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="43c52-120">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="43c52-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43c52-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43c52-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="43c52-122">Optional query parameters</span></span>

<span data-ttu-id="43c52-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="43c52-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43c52-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43c52-124">Request headers</span></span>

| <span data-ttu-id="43c52-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43c52-125">Header</span></span>       | <span data-ttu-id="43c52-126">Valor</span><span class="sxs-lookup"><span data-stu-id="43c52-126">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="43c52-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="43c52-127">Authorization</span></span>  | <span data-ttu-id="43c52-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43c52-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43c52-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43c52-130">Request body</span></span>

<span data-ttu-id="43c52-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43c52-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43c52-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="43c52-132">Response</span></span>

<span data-ttu-id="43c52-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43c52-133">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43c52-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43c52-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="43c52-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43c52-135">Request</span></span>

<span data-ttu-id="43c52-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="43c52-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="43c52-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="43c52-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="43c52-138">C#</span><span class="sxs-lookup"><span data-stu-id="43c52-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="43c52-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43c52-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="43c52-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43c52-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="43c52-141">Java</span><span class="sxs-lookup"><span data-stu-id="43c52-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="43c52-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="43c52-142">Response</span></span>

<span data-ttu-id="43c52-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43c52-143">The following is an example of the response.</span></span>
><span data-ttu-id="43c52-144">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="43c52-144">**Note**: The response object shown here might be shortened for readability.</span></span> 
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

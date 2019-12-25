---
title: Membros transitivos do grupo de lista
description: Obtenha uma lista dos membros do grupo. Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros. Essa operação é transitiva e também retornará uma lista simples de todos os membros aninhados.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5ff85a96025a605671fa0cd64a7d68c2f67ead7e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869602"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="d077d-105">Membros transitivos do grupo de lista</span><span class="sxs-lookup"><span data-stu-id="d077d-105">List group transitive members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d077d-106">Obtenha uma lista dos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="d077d-106">Get a list of the group's members.</span></span> <span data-ttu-id="d077d-107">Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="d077d-107">A group can have users, contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="d077d-108">Essa operação é transitiva e também retornará uma lista simples de todos os membros aninhados.</span><span class="sxs-lookup"><span data-stu-id="d077d-108">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="d077d-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d077d-109">Permissions</span></span>

<span data-ttu-id="d077d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d077d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d077d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d077d-112">Permission type</span></span>      | <span data-ttu-id="d077d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d077d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d077d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d077d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d077d-115">Directory. Read. All, Directory. AccessAsUser. All, User. ReadBasic. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="d077d-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="d077d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d077d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d077d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d077d-117">Not supported.</span></span>    |
|<span data-ttu-id="d077d-118">Application</span><span class="sxs-lookup"><span data-stu-id="d077d-118">Application</span></span> | <span data-ttu-id="d077d-119">Directory. Read. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="d077d-119">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="d077d-120">Observação: para listar os membros de um grupo de associação oculto, a permissão member. Read. Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="d077d-120">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="d077d-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d077d-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d077d-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d077d-122">Optional query parameters</span></span>

<span data-ttu-id="d077d-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d077d-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d077d-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d077d-124">Request headers</span></span>

| <span data-ttu-id="d077d-125">Nome</span><span class="sxs-lookup"><span data-stu-id="d077d-125">Name</span></span>       | <span data-ttu-id="d077d-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="d077d-126">Type</span></span> | <span data-ttu-id="d077d-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d077d-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d077d-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="d077d-128">Authorization</span></span>  | <span data-ttu-id="d077d-129">string</span><span class="sxs-lookup"><span data-stu-id="d077d-129">string</span></span>  | <span data-ttu-id="d077d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d077d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d077d-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d077d-132">Request body</span></span>

<span data-ttu-id="d077d-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d077d-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d077d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d077d-134">Response</span></span>

<span data-ttu-id="d077d-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d077d-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d077d-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d077d-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="d077d-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d077d-137">Request</span></span>

<span data-ttu-id="d077d-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d077d-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d077d-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="d077d-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d077d-140">C#</span><span class="sxs-lookup"><span data-stu-id="d077d-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d077d-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d077d-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d077d-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d077d-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d077d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d077d-143">Response</span></span>

<span data-ttu-id="d077d-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d077d-144">The following is an example of the response.</span></span>
><span data-ttu-id="d077d-145">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d077d-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d077d-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d077d-146">All the properties will be returned from an actual call.</span></span>
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
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

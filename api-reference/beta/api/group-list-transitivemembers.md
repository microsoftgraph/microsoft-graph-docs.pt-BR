---
title: Membros transitivos do grupo de lista
description: Obtenha uma lista dos membros do grupo. Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros. Essa operação é transitiva e também retornará uma lista simples de todos os membros aninhados.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 32c2820a0dc7f5ce690a3342da578d1fccb31bf6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419097"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="2fbaa-105">Membros transitivos do grupo de lista</span><span class="sxs-lookup"><span data-stu-id="2fbaa-105">List group transitive members</span></span>

<span data-ttu-id="2fbaa-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2fbaa-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fbaa-107">Obtenha uma lista dos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="2fbaa-107">Get a list of the group's members.</span></span> <span data-ttu-id="2fbaa-108">Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="2fbaa-108">A group can have users, contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="2fbaa-109">Essa operação é transitiva e também retornará uma lista simples de todos os membros aninhados.</span><span class="sxs-lookup"><span data-stu-id="2fbaa-109">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fbaa-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="2fbaa-110">Permissions</span></span>

<span data-ttu-id="2fbaa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fbaa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fbaa-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fbaa-113">Permission type</span></span>      | <span data-ttu-id="2fbaa-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2fbaa-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fbaa-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fbaa-115">Delegated (work or school account)</span></span> | <span data-ttu-id="2fbaa-116">Directory. Read. All, Directory. AccessAsUser. All, User. ReadBasic. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="2fbaa-116">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="2fbaa-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fbaa-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fbaa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fbaa-118">Not supported.</span></span>    |
|<span data-ttu-id="2fbaa-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fbaa-119">Application</span></span> | <span data-ttu-id="2fbaa-120">Directory. Read. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="2fbaa-120">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="2fbaa-121">Observação: para listar os membros de um grupo de associação oculto, a permissão member. Read. Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="2fbaa-121">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="2fbaa-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fbaa-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2fbaa-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2fbaa-123">Optional query parameters</span></span>

<span data-ttu-id="2fbaa-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2fbaa-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2fbaa-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fbaa-125">Request headers</span></span>

| <span data-ttu-id="2fbaa-126">Nome</span><span class="sxs-lookup"><span data-stu-id="2fbaa-126">Name</span></span>       | <span data-ttu-id="2fbaa-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fbaa-127">Type</span></span> | <span data-ttu-id="2fbaa-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fbaa-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2fbaa-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fbaa-129">Authorization</span></span>  | <span data-ttu-id="2fbaa-130">string</span><span class="sxs-lookup"><span data-stu-id="2fbaa-130">string</span></span>  | <span data-ttu-id="2fbaa-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fbaa-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2fbaa-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fbaa-133">Request body</span></span>

<span data-ttu-id="2fbaa-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2fbaa-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fbaa-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fbaa-135">Response</span></span>

<span data-ttu-id="2fbaa-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fbaa-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fbaa-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fbaa-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="2fbaa-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fbaa-138">Request</span></span>

<span data-ttu-id="2fbaa-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fbaa-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2fbaa-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fbaa-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="2fbaa-141">C#</span><span class="sxs-lookup"><span data-stu-id="2fbaa-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fbaa-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fbaa-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fbaa-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fbaa-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2fbaa-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fbaa-144">Response</span></span>

<span data-ttu-id="2fbaa-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2fbaa-145">The following is an example of the response.</span></span>
><span data-ttu-id="2fbaa-146">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2fbaa-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2fbaa-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fbaa-147">All the properties will be returned from an actual call.</span></span>
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

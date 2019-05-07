---
title: Membros transitivos do grupo de lista
description: Obtenha uma lista dos membros do grupo. Um grupo pode ter usuários, dispositivos e outros grupos como membros. Essa operação é transitiva e também retornará uma lista simples de todos os membros aninhados.
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 9c604853dcaca2f07105d3fb765c74d769836bd5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613770"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="b4514-105">Membros transitivos do grupo de lista</span><span class="sxs-lookup"><span data-stu-id="b4514-105">List group transitive members</span></span>

<span data-ttu-id="b4514-106">Obtenha uma lista dos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="b4514-106">Get a list of the group's members.</span></span> <span data-ttu-id="b4514-107">Um grupo pode ter usuários, dispositivos e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="b4514-107">A group can have users, devices and other groups as members.</span></span> <span data-ttu-id="b4514-108">Essa operação é transitiva e também retornará uma lista simples de todos os membros aninhados.</span><span class="sxs-lookup"><span data-stu-id="b4514-108">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4514-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="b4514-109">Permissions</span></span>

<span data-ttu-id="b4514-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4514-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4514-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4514-112">Permission type</span></span>      | <span data-ttu-id="b4514-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b4514-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4514-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4514-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b4514-115">Directory. Read. All, Directory. AccessAsUser. All, User. ReadBasic. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="b4514-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="b4514-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4514-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4514-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4514-117">Not supported.</span></span>    |
|<span data-ttu-id="b4514-118">Application</span><span class="sxs-lookup"><span data-stu-id="b4514-118">Application</span></span> | <span data-ttu-id="b4514-119">Directory. Read. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="b4514-119">Directory.Read.All, User.Read.All</span></span> |

><span data-ttu-id="b4514-120">**Observação:** Para listar os membros de um grupo de associação oculto, a permissão member. Read. Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="b4514-120">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="b4514-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4514-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4514-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b4514-122">Optional query parameters</span></span>

<span data-ttu-id="b4514-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b4514-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4514-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4514-124">Request headers</span></span>

| <span data-ttu-id="b4514-125">Nome</span><span class="sxs-lookup"><span data-stu-id="b4514-125">Name</span></span>       | <span data-ttu-id="b4514-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4514-126">Type</span></span> | <span data-ttu-id="b4514-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4514-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b4514-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4514-128">Authorization</span></span>  | <span data-ttu-id="b4514-129">string</span><span class="sxs-lookup"><span data-stu-id="b4514-129">string</span></span>  | <span data-ttu-id="b4514-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4514-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4514-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4514-132">Request body</span></span>

<span data-ttu-id="b4514-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b4514-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4514-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4514-134">Response</span></span>

<span data-ttu-id="b4514-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4514-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4514-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4514-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4514-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4514-137">Request</span></span>

<span data-ttu-id="b4514-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4514-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```

### <a name="response"></a><span data-ttu-id="b4514-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4514-139">Response</span></span>

<span data-ttu-id="b4514-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b4514-140">The following is an example of the response.</span></span>
><span data-ttu-id="b4514-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4514-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b4514-143">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b4514-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b4514-144">Basic</span><span class="sxs-lookup"><span data-stu-id="b4514-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_transitivemembers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4514-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4514-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_transitivemembers-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-transitivemembers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-transitivemembers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

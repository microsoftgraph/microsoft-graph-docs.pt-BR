---
title: Membros transitivos do grupo de lista
description: Obtenha uma lista dos membros do grupo. Um grupo pode ter usuários, dispositivos e outros grupos como membros. Essa operação é transitiva e também retornará uma lista simples de todos os membros aninhados.
author: anchanda
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 97959c98f7a39b27d0943fcdc57f29d181c2367d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337157"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="74c1e-105">Membros transitivos do grupo de lista</span><span class="sxs-lookup"><span data-stu-id="74c1e-105">List group transitive members</span></span>

<span data-ttu-id="74c1e-106">Obtenha uma lista dos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="74c1e-106">Get a list of the group's members.</span></span> <span data-ttu-id="74c1e-107">Um grupo pode ter usuários, dispositivos e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="74c1e-107">A group can have users, devices and other groups as members.</span></span> <span data-ttu-id="74c1e-108">Essa operação é transitiva e também retornará uma lista simples de todos os membros aninhados.</span><span class="sxs-lookup"><span data-stu-id="74c1e-108">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="74c1e-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="74c1e-109">Permissions</span></span>

<span data-ttu-id="74c1e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74c1e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74c1e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74c1e-112">Permission type</span></span>      | <span data-ttu-id="74c1e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74c1e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74c1e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74c1e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="74c1e-115">Directory. Read. All, Directory. AccessAsUser. All, User. ReadBasic. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="74c1e-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="74c1e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74c1e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74c1e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74c1e-117">Not supported.</span></span>    |
|<span data-ttu-id="74c1e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74c1e-118">Application</span></span> | <span data-ttu-id="74c1e-119">Directory. Read. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="74c1e-119">Directory.Read.All, User.Read.All</span></span> |

><span data-ttu-id="74c1e-120">**Observação:** Para listar os membros de um grupo de associação oculto, a permissão member. Read. Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="74c1e-120">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="74c1e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74c1e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="74c1e-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="74c1e-122">Optional query parameters</span></span>

<span data-ttu-id="74c1e-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="74c1e-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74c1e-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74c1e-124">Request headers</span></span>

| <span data-ttu-id="74c1e-125">Nome</span><span class="sxs-lookup"><span data-stu-id="74c1e-125">Name</span></span>       | <span data-ttu-id="74c1e-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="74c1e-126">Type</span></span> | <span data-ttu-id="74c1e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="74c1e-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="74c1e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="74c1e-128">Authorization</span></span>  | <span data-ttu-id="74c1e-129">string</span><span class="sxs-lookup"><span data-stu-id="74c1e-129">string</span></span>  | <span data-ttu-id="74c1e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74c1e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74c1e-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74c1e-132">Request body</span></span>

<span data-ttu-id="74c1e-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74c1e-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74c1e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="74c1e-134">Response</span></span>

<span data-ttu-id="74c1e-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74c1e-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74c1e-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74c1e-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="74c1e-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74c1e-137">Request</span></span>

<span data-ttu-id="74c1e-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="74c1e-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="74c1e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="74c1e-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="74c1e-140">C#</span><span class="sxs-lookup"><span data-stu-id="74c1e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74c1e-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74c1e-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="74c1e-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="74c1e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="74c1e-143">Java</span><span class="sxs-lookup"><span data-stu-id="74c1e-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="74c1e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="74c1e-144">Response</span></span>

<span data-ttu-id="74c1e-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="74c1e-145">The following is an example of the response.</span></span>
><span data-ttu-id="74c1e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74c1e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

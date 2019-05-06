---
title: Grupo de lista memberOf
description: Obter grupos e unidades administrativas dos quais o grupo é membro direto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 311837236f20039178ee4865489a83baa9fd8c1a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592935"
---
# <a name="list-group-memberof"></a><span data-ttu-id="bc9f3-103">Grupo de lista memberOf</span><span class="sxs-lookup"><span data-stu-id="bc9f3-103">List group memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc9f3-104">Obter grupos e unidades administrativas dos quais o grupo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="bc9f3-104">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="bc9f3-p101">Essa operação não é transitiva. Ao contrário de obter os grupos do Office 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="bc9f3-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="bc9f3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc9f3-107">Permissions</span></span>

<span data-ttu-id="bc9f3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc9f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc9f3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc9f3-110">Permission type</span></span>      | <span data-ttu-id="bc9f3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc9f3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc9f3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc9f3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bc9f3-113">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bc9f3-113">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bc9f3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc9f3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc9f3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc9f3-115">Not supported.</span></span>    |
|<span data-ttu-id="bc9f3-116">Application</span><span class="sxs-lookup"><span data-stu-id="bc9f3-116">Application</span></span> | <span data-ttu-id="bc9f3-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc9f3-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc9f3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc9f3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc9f3-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bc9f3-119">Optional query parameters</span></span>
<span data-ttu-id="bc9f3-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bc9f3-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc9f3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc9f3-121">Request headers</span></span>
| <span data-ttu-id="bc9f3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="bc9f3-122">Name</span></span>       | <span data-ttu-id="bc9f3-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc9f3-123">Type</span></span> | <span data-ttu-id="bc9f3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc9f3-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bc9f3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc9f3-125">Authorization</span></span>  | <span data-ttu-id="bc9f3-126">string</span><span class="sxs-lookup"><span data-stu-id="bc9f3-126">string</span></span>  | <span data-ttu-id="bc9f3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc9f3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc9f3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc9f3-129">Request body</span></span>
<span data-ttu-id="bc9f3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc9f3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc9f3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc9f3-131">Response</span></span>
<span data-ttu-id="bc9f3-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc9f3-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc9f3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc9f3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc9f3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc9f3-134">Request</span></span>

<span data-ttu-id="bc9f3-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc9f3-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="bc9f3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc9f3-136">Response</span></span>

<span data-ttu-id="bc9f3-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bc9f3-137">The following is an example of the response.</span></span>
><span data-ttu-id="bc9f3-138">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bc9f3-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bc9f3-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc9f3-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bc9f3-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="bc9f3-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bc9f3-141">Basic</span><span class="sxs-lookup"><span data-stu-id="bc9f3-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_memberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bc9f3-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc9f3-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_memberof-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-memberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-memberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

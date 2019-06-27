---
title: Listar proprietários
description: Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 4db7b27899879d6564670725fb205f4b47fa6d33
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263036"
---
# <a name="list-owners"></a><span data-ttu-id="72518-104">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="72518-104">List owners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72518-p102">Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="72518-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="72518-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="72518-107">Permissions</span></span>
<span data-ttu-id="72518-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72518-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72518-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72518-110">Permission type</span></span>      | <span data-ttu-id="72518-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72518-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72518-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72518-112">Delegated (work or school account)</span></span> | <span data-ttu-id="72518-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72518-113">Not supported.</span></span>    |
|<span data-ttu-id="72518-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72518-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72518-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72518-115">Not supported.</span></span>    |
|<span data-ttu-id="72518-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72518-116">Application</span></span> | <span data-ttu-id="72518-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72518-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72518-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72518-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72518-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="72518-119">Optional query parameters</span></span>
<span data-ttu-id="72518-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="72518-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72518-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72518-121">Request headers</span></span>
| <span data-ttu-id="72518-122">Nome</span><span class="sxs-lookup"><span data-stu-id="72518-122">Name</span></span>       | <span data-ttu-id="72518-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="72518-123">Type</span></span> | <span data-ttu-id="72518-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="72518-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="72518-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="72518-125">Authorization</span></span>  | <span data-ttu-id="72518-126">string</span><span class="sxs-lookup"><span data-stu-id="72518-126">string</span></span>  | <span data-ttu-id="72518-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72518-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72518-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72518-129">Request body</span></span>
<span data-ttu-id="72518-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72518-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72518-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="72518-131">Response</span></span>
<span data-ttu-id="72518-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72518-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72518-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72518-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="72518-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72518-134">Request</span></span>
<span data-ttu-id="72518-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="72518-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="72518-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="72518-136">Response</span></span>
<span data-ttu-id="72518-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="72518-137">The following is an example of the response.</span></span>
><span data-ttu-id="72518-138">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="72518-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="72518-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72518-139">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="72518-140">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="72518-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="72518-141">C#</span><span class="sxs-lookup"><span data-stu-id="72518-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_owners-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72518-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="72518-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_owners-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="72518-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="72518-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_owners-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-owners.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-list-owners.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-owners.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

---
title: Listar rejectedSenders
description: 'Obtenha uma lista de usuários ou grupos que estão na lista de remetentes rejeitados para este grupo. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a9d2ac3fe041e58ddba7d35d08f2f15856b2bd0d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263060"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="3c096-103">Listar rejectedSenders</span><span class="sxs-lookup"><span data-stu-id="3c096-103">List rejectedSenders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c096-104">Obtenha uma lista de usuários ou grupos que estão na lista de remetentes rejeitados para este grupo.</span><span class="sxs-lookup"><span data-stu-id="3c096-104">Get a list of users or groups that are in the rejected-senders list for this group.</span></span> 

<span data-ttu-id="3c096-p101">Os usuários na lista de remetentes rejeitados não podem postar em conversas do grupo (identificado na URL da solicitação GET). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="3c096-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c096-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c096-107">Permissions</span></span>
<span data-ttu-id="3c096-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c096-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c096-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c096-110">Permission type</span></span>      | <span data-ttu-id="3c096-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c096-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c096-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c096-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3c096-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c096-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3c096-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c096-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c096-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c096-115">Not supported.</span></span>    |
|<span data-ttu-id="3c096-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c096-116">Application</span></span> | <span data-ttu-id="3c096-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c096-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c096-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c096-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c096-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3c096-119">Optional query parameters</span></span>
<span data-ttu-id="3c096-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3c096-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c096-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c096-121">Request headers</span></span>
| <span data-ttu-id="3c096-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c096-122">Header</span></span>       | <span data-ttu-id="3c096-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3c096-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3c096-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c096-124">Authorization</span></span>  | <span data-ttu-id="3c096-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c096-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3c096-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c096-127">Request body</span></span>
<span data-ttu-id="3c096-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c096-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c096-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c096-129">Response</span></span>
<span data-ttu-id="3c096-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c096-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c096-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c096-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3c096-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c096-132">Request</span></span>
<span data-ttu-id="3c096-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c096-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/rejectedSenders
```

#### <a name="response"></a><span data-ttu-id="3c096-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c096-134">Response</span></span>
<span data-ttu-id="3c096-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c096-135">The following is an example of the response.</span></span>
><span data-ttu-id="3c096-136">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3c096-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3c096-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c096-137">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3c096-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3c096-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3c096-139">C#</span><span class="sxs-lookup"><span data-stu-id="3c096-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_rejectedsenders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c096-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c096-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_rejectedsenders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3c096-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3c096-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_rejectedsenders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-list-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

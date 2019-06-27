---
title: Delete channel
description: Exclua o canal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d1beba200c44ab74b1271a62a3c7f194a7aff279
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262203"
---
# <a name="delete-channel"></a><span data-ttu-id="38788-103">Delete channel</span><span class="sxs-lookup"><span data-stu-id="38788-103">Delete channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38788-104">Exclua o [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="38788-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="38788-105">**Observação**: Há um problema conhecido com as permissões do aplicativo e este API.</span><span class="sxs-lookup"><span data-stu-id="38788-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="38788-106">Para saber mais, confira a [lista de problemas conhecidos](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="38788-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="38788-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="38788-107">Permissions</span></span>
<span data-ttu-id="38788-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38788-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38788-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38788-110">Permission type</span></span>      | <span data-ttu-id="38788-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38788-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38788-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38788-112">Delegated (work or school account)</span></span> | <span data-ttu-id="38788-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38788-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="38788-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38788-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38788-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38788-115">Not supported.</span></span>    |
|<span data-ttu-id="38788-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38788-116">Application</span></span> | <span data-ttu-id="38788-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38788-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="38788-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="38788-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="38788-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="38788-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="38788-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38788-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="38788-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38788-121">Request headers</span></span>
| <span data-ttu-id="38788-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38788-122">Header</span></span>       | <span data-ttu-id="38788-123">Valor</span><span class="sxs-lookup"><span data-stu-id="38788-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="38788-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="38788-124">Authorization</span></span>  | <span data-ttu-id="38788-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38788-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="38788-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38788-127">Request body</span></span>
<span data-ttu-id="38788-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38788-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38788-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="38788-129">Response</span></span>

<span data-ttu-id="38788-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38788-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="38788-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38788-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38788-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38788-133">Request</span></span>
<span data-ttu-id="38788-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38788-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="38788-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="38788-135">Response</span></span>

<span data-ttu-id="38788-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="38788-136">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="38788-137">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="38788-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="38788-138">C#</span><span class="sxs-lookup"><span data-stu-id="38788-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_channel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38788-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="38788-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_channel-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="38788-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="38788-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_channel-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/channel-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

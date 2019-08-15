---
title: Delete channel
description: Exclua o canal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 41960bab36ab562dd2183374e2df5b26d96d6755
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418824"
---
# <a name="delete-channel"></a><span data-ttu-id="fb065-103">Delete channel</span><span class="sxs-lookup"><span data-stu-id="fb065-103">Delete channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb065-104">Exclua o [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="fb065-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="fb065-105">**Observação**: Há um problema conhecido com as permissões do aplicativo e este API.</span><span class="sxs-lookup"><span data-stu-id="fb065-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="fb065-106">Para saber mais, confira a [lista de problemas conhecidos](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="fb065-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="fb065-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb065-107">Permissions</span></span>
<span data-ttu-id="fb065-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb065-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb065-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb065-110">Permission type</span></span>      | <span data-ttu-id="fb065-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb065-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb065-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb065-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fb065-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb065-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fb065-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb065-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb065-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb065-115">Not supported.</span></span>    |
|<span data-ttu-id="fb065-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb065-116">Application</span></span> | <span data-ttu-id="fb065-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb065-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="fb065-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="fb065-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="fb065-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="fb065-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="fb065-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb065-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fb065-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb065-121">Request headers</span></span>
| <span data-ttu-id="fb065-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb065-122">Header</span></span>       | <span data-ttu-id="fb065-123">Valor</span><span class="sxs-lookup"><span data-stu-id="fb065-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fb065-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb065-124">Authorization</span></span>  | <span data-ttu-id="fb065-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb065-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fb065-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb065-127">Request body</span></span>
<span data-ttu-id="fb065-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fb065-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb065-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb065-129">Response</span></span>

<span data-ttu-id="fb065-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb065-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fb065-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb065-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb065-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb065-133">Request</span></span>
<span data-ttu-id="fb065-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb065-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fb065-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb065-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fb065-136">C#</span><span class="sxs-lookup"><span data-stu-id="fb065-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fb065-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb065-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fb065-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fb065-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fb065-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb065-139">Response</span></span>

<span data-ttu-id="fb065-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fb065-140">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->

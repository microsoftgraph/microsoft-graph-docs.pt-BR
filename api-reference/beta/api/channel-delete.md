---
title: Delete channel
description: Exclua o canal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6e0204fea1a3291bbca4c942a03e5364fc5b4a47
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983286"
---
# <a name="delete-channel"></a><span data-ttu-id="e5ff5-103">Delete channel</span><span class="sxs-lookup"><span data-stu-id="e5ff5-103">Delete channel</span></span>

<span data-ttu-id="e5ff5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5ff5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5ff5-105">Exclua o [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="e5ff5-105">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="e5ff5-106">**Observação**: Há um problema conhecido com as permissões do aplicativo e este API.</span><span class="sxs-lookup"><span data-stu-id="e5ff5-106">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="e5ff5-107">Para saber mais, confira a [lista de problemas conhecidos](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="e5ff5-107">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="e5ff5-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5ff5-108">Permissions</span></span>
<span data-ttu-id="e5ff5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5ff5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5ff5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5ff5-111">Permission type</span></span>      | <span data-ttu-id="e5ff5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5ff5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5ff5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5ff5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e5ff5-114">Channel. Delete. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e5ff5-114">Channel.Delete.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="e5ff5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5ff5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5ff5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5ff5-116">Not supported.</span></span>    |
|<span data-ttu-id="e5ff5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5ff5-117">Application</span></span> | <span data-ttu-id="e5ff5-118">Channel. Delete. All, Channel. Delete. Group \*, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e5ff5-118">Channel.Delete.All, Channel.Delete.Group\*, Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |

> <span data-ttu-id="e5ff5-119">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="e5ff5-119">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="e5ff5-120">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="e5ff5-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e5ff5-121">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="e5ff5-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e5ff5-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5ff5-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e5ff5-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5ff5-123">Request headers</span></span>
| <span data-ttu-id="e5ff5-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e5ff5-124">Header</span></span>       | <span data-ttu-id="e5ff5-125">Valor</span><span class="sxs-lookup"><span data-stu-id="e5ff5-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e5ff5-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5ff5-126">Authorization</span></span>  | <span data-ttu-id="e5ff5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5ff5-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e5ff5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5ff5-129">Request body</span></span>
<span data-ttu-id="e5ff5-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5ff5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5ff5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5ff5-131">Response</span></span>

<span data-ttu-id="e5ff5-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5ff5-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e5ff5-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5ff5-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5ff5-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5ff5-135">Request</span></span>
<span data-ttu-id="e5ff5-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5ff5-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e5ff5-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5ff5-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="c"></a>[<span data-ttu-id="e5ff5-138">C#</span><span class="sxs-lookup"><span data-stu-id="e5ff5-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5ff5-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5ff5-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5ff5-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5ff5-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e5ff5-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5ff5-141">Response</span></span>

<span data-ttu-id="e5ff5-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5ff5-142">The following is an example of the response.</span></span> 
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



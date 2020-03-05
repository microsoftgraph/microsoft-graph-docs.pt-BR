---
title: Delete channel
description: Exclua o canal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 63ec098bab921edcdb3eeabe9d2ec4efda62b6ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440448"
---
# <a name="delete-channel"></a><span data-ttu-id="634fa-103">Delete channel</span><span class="sxs-lookup"><span data-stu-id="634fa-103">Delete channel</span></span>

<span data-ttu-id="634fa-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="634fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="634fa-105">Exclua o [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="634fa-105">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="634fa-106">**Observação**: Há um problema conhecido com as permissões do aplicativo e este API.</span><span class="sxs-lookup"><span data-stu-id="634fa-106">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="634fa-107">Para saber mais, confira a [lista de problemas conhecidos](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="634fa-107">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="634fa-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="634fa-108">Permissions</span></span>
<span data-ttu-id="634fa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="634fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="634fa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="634fa-111">Permission type</span></span>      | <span data-ttu-id="634fa-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="634fa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="634fa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="634fa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="634fa-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="634fa-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="634fa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="634fa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="634fa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="634fa-116">Not supported.</span></span>    |
|<span data-ttu-id="634fa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="634fa-117">Application</span></span> | <span data-ttu-id="634fa-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="634fa-118">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="634fa-119">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="634fa-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="634fa-120">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="634fa-120">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="634fa-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="634fa-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="634fa-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="634fa-122">Request headers</span></span>
| <span data-ttu-id="634fa-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="634fa-123">Header</span></span>       | <span data-ttu-id="634fa-124">Valor</span><span class="sxs-lookup"><span data-stu-id="634fa-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="634fa-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="634fa-125">Authorization</span></span>  | <span data-ttu-id="634fa-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="634fa-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="634fa-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="634fa-128">Request body</span></span>
<span data-ttu-id="634fa-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="634fa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="634fa-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="634fa-130">Response</span></span>

<span data-ttu-id="634fa-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="634fa-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="634fa-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="634fa-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="634fa-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="634fa-134">Request</span></span>
<span data-ttu-id="634fa-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="634fa-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="634fa-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="634fa-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="c"></a>[<span data-ttu-id="634fa-137">C#</span><span class="sxs-lookup"><span data-stu-id="634fa-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="634fa-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="634fa-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="634fa-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="634fa-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="634fa-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="634fa-140">Response</span></span>

<span data-ttu-id="634fa-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="634fa-141">The following is an example of the response.</span></span> 
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

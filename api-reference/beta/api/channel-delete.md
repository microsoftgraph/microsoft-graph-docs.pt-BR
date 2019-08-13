---
title: Delete channel
description: Exclua o canal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0818eb1cdc96e6c6b9642b122829b2fac6e6f9e9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317552"
---
# <a name="delete-channel"></a><span data-ttu-id="00c38-103">Delete channel</span><span class="sxs-lookup"><span data-stu-id="00c38-103">Delete channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00c38-104">Exclua o [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="00c38-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="00c38-105">**Observação**: Há um problema conhecido com as permissões do aplicativo e este API.</span><span class="sxs-lookup"><span data-stu-id="00c38-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="00c38-106">Para saber mais, confira a [lista de problemas conhecidos](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="00c38-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="00c38-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="00c38-107">Permissions</span></span>
<span data-ttu-id="00c38-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00c38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00c38-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00c38-110">Permission type</span></span>      | <span data-ttu-id="00c38-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00c38-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00c38-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00c38-112">Delegated (work or school account)</span></span> | <span data-ttu-id="00c38-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00c38-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="00c38-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00c38-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00c38-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00c38-115">Not supported.</span></span>    |
|<span data-ttu-id="00c38-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00c38-116">Application</span></span> | <span data-ttu-id="00c38-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00c38-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="00c38-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="00c38-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="00c38-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="00c38-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="00c38-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00c38-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="00c38-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00c38-121">Request headers</span></span>
| <span data-ttu-id="00c38-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="00c38-122">Header</span></span>       | <span data-ttu-id="00c38-123">Valor</span><span class="sxs-lookup"><span data-stu-id="00c38-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="00c38-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="00c38-124">Authorization</span></span>  | <span data-ttu-id="00c38-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00c38-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="00c38-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00c38-127">Request body</span></span>
<span data-ttu-id="00c38-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="00c38-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00c38-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="00c38-129">Response</span></span>

<span data-ttu-id="00c38-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00c38-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="00c38-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00c38-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00c38-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00c38-133">Request</span></span>
<span data-ttu-id="00c38-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="00c38-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="00c38-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="00c38-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="00c38-136">C#</span><span class="sxs-lookup"><span data-stu-id="00c38-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00c38-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00c38-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="00c38-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="00c38-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="00c38-139">Java</span><span class="sxs-lookup"><span data-stu-id="00c38-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="00c38-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="00c38-140">Response</span></span>

<span data-ttu-id="00c38-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="00c38-141">The following is an example of the response.</span></span> 
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

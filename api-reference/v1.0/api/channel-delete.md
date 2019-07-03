---
title: Delete channel
description: Exclua o canal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c4d710ad9acdd176a13ca382aefe7d67441fe02a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443704"
---
# <a name="delete-channel"></a><span data-ttu-id="95fc5-103">Delete channel</span><span class="sxs-lookup"><span data-stu-id="95fc5-103">Delete channel</span></span>



<span data-ttu-id="95fc5-104">Exclua o [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="95fc5-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="95fc5-105">**Observação**: Há um problema conhecido com as permissões do aplicativo e este API.</span><span class="sxs-lookup"><span data-stu-id="95fc5-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="95fc5-106">Para saber mais, confira a [lista de problemas conhecidos](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="95fc5-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

> <span data-ttu-id="95fc5-107">**Observação**: os dados nos canais excluídos continuarão a ser armazenados por várias semanas para permitir que o proprietário da equipe retenha o canal excluído.</span><span class="sxs-lookup"><span data-stu-id="95fc5-107">**Note**: The data in deleted channels will continue to be stored for several weeks to allow team owner to recovery deleted channel.</span></span> <span data-ttu-id="95fc5-108">Durante esse tempo, um novo canal com o mesmo displayName não pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="95fc5-108">During that time, a new channel with the same displayName may not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="95fc5-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="95fc5-109">Permissions</span></span>
<span data-ttu-id="95fc5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95fc5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95fc5-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95fc5-112">Permission type</span></span>      | <span data-ttu-id="95fc5-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95fc5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95fc5-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95fc5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="95fc5-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95fc5-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="95fc5-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95fc5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95fc5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95fc5-117">Not supported.</span></span>    |
|<span data-ttu-id="95fc5-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95fc5-118">Application</span></span> | <span data-ttu-id="95fc5-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95fc5-119">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="95fc5-120">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="95fc5-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="95fc5-121">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="95fc5-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="95fc5-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95fc5-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="95fc5-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95fc5-123">Request headers</span></span>
| <span data-ttu-id="95fc5-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95fc5-124">Header</span></span>       | <span data-ttu-id="95fc5-125">Valor</span><span class="sxs-lookup"><span data-stu-id="95fc5-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="95fc5-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="95fc5-126">Authorization</span></span>  | <span data-ttu-id="95fc5-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95fc5-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="95fc5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95fc5-129">Request body</span></span>
<span data-ttu-id="95fc5-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95fc5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95fc5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="95fc5-131">Response</span></span>

<span data-ttu-id="95fc5-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95fc5-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="95fc5-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95fc5-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95fc5-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95fc5-135">Request</span></span>
<span data-ttu-id="95fc5-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="95fc5-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="95fc5-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="95fc5-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="95fc5-138">C#</span><span class="sxs-lookup"><span data-stu-id="95fc5-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="95fc5-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="95fc5-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="95fc5-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="95fc5-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="95fc5-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="95fc5-141">Response</span></span>

<span data-ttu-id="95fc5-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="95fc5-142">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

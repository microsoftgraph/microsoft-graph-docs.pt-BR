---
title: Criar acceptedSender
description: Adicione um novo usuário ou grupo à lista acceptedSender.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 6f557cd1d4884f765334abe394610c520db68ead
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329735"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="bb0f6-103">Criar acceptedSender</span><span class="sxs-lookup"><span data-stu-id="bb0f6-103">Create acceptedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb0f6-104">Adicione um novo usuário ou grupo à lista acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="bb0f6-104">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="bb0f6-p101">Especifique o usuário ou grupo em `@odata.id` no corpo da solicitação. Os usuários na lista de remetentes aceitos podem postar em conversas do grupo. Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="bb0f6-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb0f6-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb0f6-108">Permissions</span></span>
<span data-ttu-id="bb0f6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb0f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb0f6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb0f6-111">Permission type</span></span>      | <span data-ttu-id="bb0f6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb0f6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb0f6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb0f6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bb0f6-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb0f6-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bb0f6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb0f6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb0f6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb0f6-116">Not supported.</span></span>    |
|<span data-ttu-id="bb0f6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb0f6-117">Application</span></span> | <span data-ttu-id="bb0f6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb0f6-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb0f6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb0f6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="bb0f6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb0f6-120">Request headers</span></span>
| <span data-ttu-id="bb0f6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb0f6-121">Header</span></span>       | <span data-ttu-id="bb0f6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bb0f6-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bb0f6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb0f6-123">Authorization</span></span>  | <span data-ttu-id="bb0f6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb0f6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bb0f6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb0f6-126">Request body</span></span>
<span data-ttu-id="bb0f6-127">No corpo da solicitação, forneça a id de um objeto de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="bb0f6-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="bb0f6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb0f6-128">Response</span></span>
<span data-ttu-id="bb0f6-129">Este método retorna o código de resposta `204 No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bb0f6-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb0f6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb0f6-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bb0f6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb0f6-131">Request</span></span>
<span data-ttu-id="bb0f6-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb0f6-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_acceptedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```

#### <a name="response"></a><span data-ttu-id="bb0f6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb0f6-133">Response</span></span>
<span data-ttu-id="bb0f6-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bb0f6-134">The following is an example of the response.</span></span>
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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

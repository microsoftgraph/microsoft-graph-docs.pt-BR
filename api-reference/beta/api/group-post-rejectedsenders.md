---
title: Criar rejectedSender
description: Adiciona um novo usuário ou grupo à lista rejectedSender.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: d1f22c5a14a9d08204532217d61665659acc979a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328516"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="b3fc2-103">Criar rejectedSender</span><span class="sxs-lookup"><span data-stu-id="b3fc2-103">Create rejectedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3fc2-104">Adiciona um novo usuário ou grupo à lista rejectedSender.</span><span class="sxs-lookup"><span data-stu-id="b3fc2-104">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="b3fc2-p101">Especifique o usuário ou grupo em `@odata.id` no corpo da solicitação. Os usuários na lista de remetentes rejeitados não podem postar em conversas do grupo (identificado na URL da solicitação POST). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="b3fc2-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3fc2-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3fc2-108">Permissions</span></span>
<span data-ttu-id="b3fc2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3fc2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3fc2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3fc2-111">Permission type</span></span>      | <span data-ttu-id="b3fc2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3fc2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3fc2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3fc2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b3fc2-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3fc2-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b3fc2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3fc2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3fc2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3fc2-116">Not supported.</span></span>    |
|<span data-ttu-id="b3fc2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3fc2-117">Application</span></span> | <span data-ttu-id="b3fc2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3fc2-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3fc2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3fc2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b3fc2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3fc2-120">Request headers</span></span>
| <span data-ttu-id="b3fc2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3fc2-121">Header</span></span>       | <span data-ttu-id="b3fc2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b3fc2-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b3fc2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3fc2-123">Authorization</span></span>  | <span data-ttu-id="b3fc2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3fc2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b3fc2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3fc2-126">Request body</span></span>
<span data-ttu-id="b3fc2-127">No corpo da solicitação, forneça a id de um objeto de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="b3fc2-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="b3fc2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3fc2-128">Response</span></span>
<span data-ttu-id="b3fc2-129">Este método retorna o código de resposta `204 No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3fc2-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3fc2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3fc2-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b3fc2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3fc2-131">Request</span></span>
<span data-ttu-id="b3fc2-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3fc2-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rejectedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```

#### <a name="response"></a><span data-ttu-id="b3fc2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3fc2-133">Response</span></span>
<span data-ttu-id="b3fc2-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3fc2-134">The following is an example of the response.</span></span>
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
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

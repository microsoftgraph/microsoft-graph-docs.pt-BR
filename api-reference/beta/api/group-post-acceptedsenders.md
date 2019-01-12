---
title: Criar acceptedSender
description: Adicione um novo usuário ou grupo à lista acceptedSender.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 650e0902b7968cd920e4148fddd0fd627e138b4c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955559"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="e8f56-103">Criar acceptedSender</span><span class="sxs-lookup"><span data-stu-id="e8f56-103">Create acceptedSender</span></span>

> <span data-ttu-id="e8f56-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e8f56-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8f56-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e8f56-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8f56-106">Adicione um novo usuário ou grupo à lista acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="e8f56-106">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="e8f56-p102">Especifique o usuário ou grupo em `@odata.id` no corpo da solicitação. Os usuários na lista de remetentes aceitos podem postar em conversas do grupo. Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="e8f56-p102">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8f56-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8f56-110">Permissions</span></span>
<span data-ttu-id="e8f56-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8f56-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8f56-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8f56-113">Permission type</span></span>      | <span data-ttu-id="e8f56-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8f56-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8f56-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8f56-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e8f56-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8f56-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8f56-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8f56-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8f56-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8f56-118">Not supported.</span></span>    |
|<span data-ttu-id="e8f56-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8f56-119">Application</span></span> | <span data-ttu-id="e8f56-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8f56-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8f56-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8f56-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e8f56-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8f56-122">Request headers</span></span>
| <span data-ttu-id="e8f56-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8f56-123">Header</span></span>       | <span data-ttu-id="e8f56-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e8f56-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e8f56-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8f56-125">Authorization</span></span>  | <span data-ttu-id="e8f56-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8f56-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e8f56-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8f56-128">Request body</span></span>
<span data-ttu-id="e8f56-129">No corpo da solicitação, forneça a id de um objeto de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="e8f56-129">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="e8f56-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8f56-130">Response</span></span>
<span data-ttu-id="e8f56-131">Este método retorna o código de resposta `204 No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e8f56-131">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8f56-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8f56-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e8f56-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8f56-133">Request</span></span>
<span data-ttu-id="e8f56-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8f56-134">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="e8f56-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8f56-135">Response</span></span>
<span data-ttu-id="e8f56-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e8f56-136">The following is an example of the response.</span></span>
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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

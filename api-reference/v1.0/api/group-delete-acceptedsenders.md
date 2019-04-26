---
title: Remover acceptedSender
description: 'Remover um usuário ou grupo da lista de remetentes aceitos. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: cf15c26fbd73501496ad11f443b20569c7801e9b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334475"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="b3e3e-103">Remover acceptedSender</span><span class="sxs-lookup"><span data-stu-id="b3e3e-103">Remove acceptedSender</span></span>
<span data-ttu-id="b3e3e-104">Remover um usuário ou grupo da lista de remetentes aceitos.</span><span class="sxs-lookup"><span data-stu-id="b3e3e-104">Remove a user or group from the accepted-senders list.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b3e3e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3e3e-105">Permissions</span></span>
<span data-ttu-id="b3e3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3e3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3e3e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3e3e-108">Permission type</span></span>                        | <span data-ttu-id="b3e3e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3e3e-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="b3e3e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3e3e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3e3e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3e3e-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="b3e3e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3e3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3e3e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3e3e-113">Not supported.</span></span> |
| <span data-ttu-id="b3e3e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3e3e-114">Application</span></span>                            | <span data-ttu-id="b3e3e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3e3e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3e3e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3e3e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
DELETE /groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/groups/{other-group-id}
```

## <a name="request-headers"></a><span data-ttu-id="b3e3e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3e3e-117">Request headers</span></span>
| <span data-ttu-id="b3e3e-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3e3e-118">Header</span></span>         | <span data-ttu-id="b3e3e-119">Valor</span><span class="sxs-lookup"><span data-stu-id="b3e3e-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="b3e3e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3e3e-120">Authorization</span></span>  | <span data-ttu-id="b3e3e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3e3e-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="b3e3e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3e3e-123">Request body</span></span>
<span data-ttu-id="b3e3e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3e3e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3e3e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3e3e-125">Response</span></span>
<span data-ttu-id="b3e3e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3e3e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3e3e-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3e3e-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b3e3e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3e3e-129">Request</span></span>
<span data-ttu-id="b3e3e-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3e3e-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="b3e3e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3e3e-131">Response</span></span>
<span data-ttu-id="b3e3e-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3e3e-132">The following is an example of the response.</span></span> 

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

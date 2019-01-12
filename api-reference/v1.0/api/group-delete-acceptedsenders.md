---
title: Remover acceptedSender
description: 'Remova um usuário ou grupo da lista acceptedSenders. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 86d9cc6cd0adf1c29f64044299daa1ed2c8403d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962363"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="56956-103">Remover acceptedSender</span><span class="sxs-lookup"><span data-stu-id="56956-103">Remove acceptedSender</span></span>
<span data-ttu-id="56956-104">Remova um usuário ou grupo da lista acceptedSenders.</span><span class="sxs-lookup"><span data-stu-id="56956-104">Remove a user or group from the acceptedSenders list.</span></span> 

## <a name="permissions"></a><span data-ttu-id="56956-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="56956-105">Permissions</span></span>
<span data-ttu-id="56956-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56956-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56956-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56956-108">Permission type</span></span>                        | <span data-ttu-id="56956-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56956-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="56956-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56956-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="56956-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56956-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="56956-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56956-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56956-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56956-113">Not supported.</span></span> |
| <span data-ttu-id="56956-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56956-114">Application</span></span>                            | <span data-ttu-id="56956-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56956-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56956-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56956-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
DELETE /groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/groups/{other-group-id}
```

## <a name="request-headers"></a><span data-ttu-id="56956-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56956-117">Request headers</span></span>
| <span data-ttu-id="56956-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56956-118">Header</span></span>         | <span data-ttu-id="56956-119">Valor</span><span class="sxs-lookup"><span data-stu-id="56956-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="56956-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="56956-120">Authorization</span></span>  | <span data-ttu-id="56956-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56956-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="56956-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56956-123">Request body</span></span>
<span data-ttu-id="56956-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="56956-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56956-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="56956-125">Response</span></span>
<span data-ttu-id="56956-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56956-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56956-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56956-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="56956-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56956-129">Request</span></span>
<span data-ttu-id="56956-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="56956-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="56956-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="56956-131">Response</span></span>
<span data-ttu-id="56956-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="56956-132">The following is an example of the response.</span></span> 

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

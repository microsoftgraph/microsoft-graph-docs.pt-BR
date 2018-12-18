---
title: Remover rejectedSender
description: Remove um usuário ou grupo da lista rejectedSenders.
author: dkershaw10
ms.openlocfilehash: cd84f14f15288207ff8c3362ea0295ae3eba1856
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311253"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="e273e-103">Remover rejectedSender</span><span class="sxs-lookup"><span data-stu-id="e273e-103">Remove rejectedSender</span></span>

> <span data-ttu-id="e273e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e273e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e273e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e273e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e273e-106">Remove um usuário ou grupo da lista rejectedSenders.</span><span class="sxs-lookup"><span data-stu-id="e273e-106">Remove a user or group from the rejectedSenders list.</span></span>

## <a name="permissions"></a><span data-ttu-id="e273e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e273e-107">Permissions</span></span>
<span data-ttu-id="e273e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e273e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e273e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e273e-110">Permission type</span></span>                        | <span data-ttu-id="e273e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e273e-111">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="e273e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e273e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e273e-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e273e-113">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="e273e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e273e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e273e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e273e-115">Not supported.</span></span> |
| <span data-ttu-id="e273e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e273e-116">Application</span></span>                            | <span data-ttu-id="e273e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e273e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e273e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e273e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id=<id>
```

## <a name="request-headers"></a><span data-ttu-id="e273e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e273e-119">Request headers</span></span>

| <span data-ttu-id="e273e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e273e-120">Header</span></span>         | <span data-ttu-id="e273e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e273e-121">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="e273e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e273e-122">Authorization</span></span>  | <span data-ttu-id="e273e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e273e-p103">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="e273e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e273e-125">Request body</span></span>
<span data-ttu-id="e273e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e273e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e273e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e273e-127">Response</span></span>
<span data-ttu-id="e273e-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e273e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e273e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e273e-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e273e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e273e-131">Request</span></span>
<span data-ttu-id="e273e-132">Estes são alguns exemplos de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e273e-132">The following are a couple of examples of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "remove_rejectedSender_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}

DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="e273e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e273e-133">Response</span></span>
<span data-ttu-id="e273e-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e273e-134">The following is an example of the response.</span></span> 
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
  "description": "Remove rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
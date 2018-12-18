---
title: Excluir conversa
description: Exclua uma conversa.
author: dkershaw10
ms.openlocfilehash: 2d35472f611b6f49ba1683ba127444d91753fac7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335746"
---
# <a name="delete-conversation"></a><span data-ttu-id="eb595-103">Excluir conversa</span><span class="sxs-lookup"><span data-stu-id="eb595-103">Delete conversation</span></span>

<span data-ttu-id="eb595-104">Exclua uma conversa.</span><span class="sxs-lookup"><span data-stu-id="eb595-104">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="eb595-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb595-105">Permissions</span></span>
<span data-ttu-id="eb595-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb595-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb595-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb595-108">Permission type</span></span>      | <span data-ttu-id="eb595-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb595-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb595-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb595-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eb595-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb595-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb595-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb595-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb595-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb595-113">Not supported.</span></span>    |
|<span data-ttu-id="eb595-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb595-114">Application</span></span> | <span data-ttu-id="eb595-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb595-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb595-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb595-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="eb595-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb595-117">Request headers</span></span>
| <span data-ttu-id="eb595-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb595-118">Header</span></span>       | <span data-ttu-id="eb595-119">Valor</span><span class="sxs-lookup"><span data-stu-id="eb595-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eb595-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb595-120">Authorization</span></span>  | <span data-ttu-id="eb595-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb595-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eb595-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb595-123">Request body</span></span>
<span data-ttu-id="eb595-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb595-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb595-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb595-125">Response</span></span>

<span data-ttu-id="eb595-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb595-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb595-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb595-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb595-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb595-129">Request</span></span>
<span data-ttu-id="eb595-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb595-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="eb595-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb595-131">Response</span></span>
<span data-ttu-id="eb595-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb595-132">Here is an example of the response.</span></span> 
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

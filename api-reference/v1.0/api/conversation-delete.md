---
title: Excluir conversa
description: Exclua uma conversa.
ms.openlocfilehash: a6fee14c0debde4ac09d6c7c7814370ecdb06c08
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005001"
---
# <a name="delete-conversation"></a><span data-ttu-id="f3630-103">Excluir conversa</span><span class="sxs-lookup"><span data-stu-id="f3630-103">Delete conversation</span></span>

<span data-ttu-id="f3630-104">Exclua uma conversa.</span><span class="sxs-lookup"><span data-stu-id="f3630-104">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="f3630-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3630-105">Permissions</span></span>
<span data-ttu-id="f3630-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3630-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3630-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3630-108">Permission type</span></span>      | <span data-ttu-id="f3630-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3630-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3630-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3630-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f3630-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3630-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f3630-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3630-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3630-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3630-113">Not supported.</span></span>    |
|<span data-ttu-id="f3630-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3630-114">Application</span></span> | <span data-ttu-id="f3630-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3630-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3630-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3630-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f3630-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3630-117">Request headers</span></span>
| <span data-ttu-id="f3630-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f3630-118">Header</span></span>       | <span data-ttu-id="f3630-119">Valor</span><span class="sxs-lookup"><span data-stu-id="f3630-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f3630-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3630-120">Authorization</span></span>  | <span data-ttu-id="f3630-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3630-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f3630-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3630-123">Request body</span></span>
<span data-ttu-id="f3630-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3630-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3630-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3630-125">Response</span></span>

<span data-ttu-id="f3630-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3630-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3630-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3630-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3630-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3630-129">Request</span></span>
<span data-ttu-id="f3630-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3630-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="f3630-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3630-131">Response</span></span>
<span data-ttu-id="f3630-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3630-132">Here is an example of the response.</span></span> 
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

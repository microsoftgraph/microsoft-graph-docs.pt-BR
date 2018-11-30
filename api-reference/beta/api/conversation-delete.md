---
title: Excluir conversa
description: Exclua uma conversa.
ms.openlocfilehash: 9a6e590470343afd7990d6f24672fe1824c65a90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035931"
---
# <a name="delete-conversation"></a><span data-ttu-id="b1160-103">Excluir conversa</span><span class="sxs-lookup"><span data-stu-id="b1160-103">Delete conversation</span></span>

> <span data-ttu-id="b1160-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b1160-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1160-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b1160-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1160-106">Exclua uma conversa.</span><span class="sxs-lookup"><span data-stu-id="b1160-106">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="b1160-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1160-107">Permissions</span></span>
<span data-ttu-id="b1160-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1160-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1160-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1160-110">Permission type</span></span>      | <span data-ttu-id="b1160-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1160-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1160-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1160-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b1160-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1160-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1160-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1160-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1160-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1160-115">Not supported.</span></span>    |
|<span data-ttu-id="b1160-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1160-116">Application</span></span> | <span data-ttu-id="b1160-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1160-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1160-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1160-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b1160-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1160-119">Request headers</span></span>
| <span data-ttu-id="b1160-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1160-120">Header</span></span>       | <span data-ttu-id="b1160-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b1160-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b1160-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1160-122">Authorization</span></span>  | <span data-ttu-id="b1160-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1160-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1160-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1160-125">Request body</span></span>
<span data-ttu-id="b1160-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b1160-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1160-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1160-127">Response</span></span>

<span data-ttu-id="b1160-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1160-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1160-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1160-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1160-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1160-131">Request</span></span>
<span data-ttu-id="b1160-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1160-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="b1160-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1160-133">Response</span></span>
<span data-ttu-id="b1160-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1160-134">Here is an example of the response.</span></span> 
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

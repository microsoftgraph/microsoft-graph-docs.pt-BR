---
title: Excluir conversationThread
description: Exclua um conversationThread.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 15e7a7aaf2b8d91a14830b40a61568501cca41b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813479"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="6c9d8-103">Excluir conversationThread</span><span class="sxs-lookup"><span data-stu-id="6c9d8-103">Delete conversationThread</span></span>

> <span data-ttu-id="6c9d8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6c9d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c9d8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6c9d8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c9d8-106">Exclua um conversationThread.</span><span class="sxs-lookup"><span data-stu-id="6c9d8-106">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="6c9d8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c9d8-107">Permissions</span></span>
<span data-ttu-id="6c9d8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c9d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c9d8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c9d8-110">Permission type</span></span>      | <span data-ttu-id="6c9d8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c9d8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c9d8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c9d8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6c9d8-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c9d8-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6c9d8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c9d8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c9d8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c9d8-115">Not supported.</span></span>    |
|<span data-ttu-id="6c9d8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c9d8-116">Application</span></span> | <span data-ttu-id="6c9d8-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c9d8-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c9d8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c9d8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="6c9d8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c9d8-119">Request headers</span></span>
| <span data-ttu-id="6c9d8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c9d8-120">Header</span></span>       | <span data-ttu-id="6c9d8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6c9d8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6c9d8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c9d8-122">Authorization</span></span>  | <span data-ttu-id="6c9d8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c9d8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6c9d8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c9d8-125">Request body</span></span>
<span data-ttu-id="6c9d8-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6c9d8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c9d8-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c9d8-127">Response</span></span>

<span data-ttu-id="6c9d8-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c9d8-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c9d8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c9d8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6c9d8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c9d8-131">Request</span></span>
<span data-ttu-id="6c9d8-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c9d8-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="6c9d8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c9d8-133">Response</span></span>
<span data-ttu-id="6c9d8-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c9d8-134">Here is an example of the response.</span></span> 
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
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

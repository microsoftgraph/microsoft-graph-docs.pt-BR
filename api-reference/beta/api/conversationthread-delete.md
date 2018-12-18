---
title: Excluir conversationThread
description: Exclua um conversationThread.
author: dkershaw10
ms.openlocfilehash: ef0f9e4eae22058c93b093a2758819e60299d4fa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316454"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="e5f0e-103">Excluir conversationThread</span><span class="sxs-lookup"><span data-stu-id="e5f0e-103">Delete conversationThread</span></span>

> <span data-ttu-id="e5f0e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e5f0e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5f0e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e5f0e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5f0e-106">Exclua um conversationThread.</span><span class="sxs-lookup"><span data-stu-id="e5f0e-106">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5f0e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5f0e-107">Permissions</span></span>
<span data-ttu-id="e5f0e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5f0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5f0e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5f0e-110">Permission type</span></span>      | <span data-ttu-id="e5f0e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5f0e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5f0e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5f0e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e5f0e-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5f0e-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e5f0e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5f0e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5f0e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5f0e-115">Not supported.</span></span>    |
|<span data-ttu-id="e5f0e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5f0e-116">Application</span></span> | <span data-ttu-id="e5f0e-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5f0e-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5f0e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5f0e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e5f0e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5f0e-119">Request headers</span></span>
| <span data-ttu-id="e5f0e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e5f0e-120">Header</span></span>       | <span data-ttu-id="e5f0e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e5f0e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e5f0e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5f0e-122">Authorization</span></span>  | <span data-ttu-id="e5f0e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5f0e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e5f0e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5f0e-125">Request body</span></span>
<span data-ttu-id="e5f0e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5f0e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5f0e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5f0e-127">Response</span></span>

<span data-ttu-id="e5f0e-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5f0e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5f0e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5f0e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5f0e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5f0e-131">Request</span></span>
<span data-ttu-id="e5f0e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5f0e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="e5f0e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5f0e-133">Response</span></span>
<span data-ttu-id="e5f0e-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5f0e-134">Here is an example of the response.</span></span> 
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
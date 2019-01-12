---
title: Excluir outlookTaskGroup
description: Exclua o outlookTaskGroup especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1ceffb66dbab189331ec4bcd500e84b79f3d341f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945570"
---
# <a name="delete-outlooktaskgroup"></a><span data-ttu-id="e5351-103">Excluir outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="e5351-103">Delete outlookTaskGroup</span></span>

> <span data-ttu-id="e5351-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e5351-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5351-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e5351-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5351-106">Exclua o especificado [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="e5351-106">Delete the specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="e5351-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e5351-107">Permissions</span></span>
<span data-ttu-id="e5351-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5351-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5351-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5351-110">Permission type</span></span>      | <span data-ttu-id="e5351-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5351-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5351-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5351-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e5351-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5351-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="e5351-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5351-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5351-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5351-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="e5351-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5351-116">Application</span></span> | <span data-ttu-id="e5351-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5351-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5351-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5351-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e5351-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5351-119">Request headers</span></span>
| <span data-ttu-id="e5351-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e5351-120">Name</span></span>       | <span data-ttu-id="e5351-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5351-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e5351-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5351-122">Authorization</span></span>  | <span data-ttu-id="e5351-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5351-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5351-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5351-125">Request body</span></span>
<span data-ttu-id="e5351-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5351-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5351-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5351-127">Response</span></span>

<span data-ttu-id="e5351-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5351-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5351-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5351-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5351-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5351-131">Request</span></span>
<span data-ttu-id="e5351-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5351-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskgroups('AAMkADIyAAAhrbe-AAA=')
```
##### <a name="response"></a><span data-ttu-id="e5351-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5351-133">Response</span></span>
<span data-ttu-id="e5351-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5351-134">Here is an example of the response.</span></span>
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
  "description": "Delete outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

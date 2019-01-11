---
title: Excluir outlookTaskGroup
description: Exclua o outlookTaskGroup especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 9cf370e04da89cf5f561ebb9aa720f507ca87a55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843180"
---
# <a name="delete-outlooktaskgroup"></a><span data-ttu-id="2096c-103">Excluir outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="2096c-103">Delete outlookTaskGroup</span></span>

> <span data-ttu-id="2096c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2096c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2096c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2096c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2096c-106">Exclua o especificado [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="2096c-106">Delete the specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="2096c-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="2096c-107">Permissions</span></span>
<span data-ttu-id="2096c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2096c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2096c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2096c-110">Permission type</span></span>      | <span data-ttu-id="2096c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2096c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2096c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2096c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2096c-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2096c-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="2096c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2096c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2096c-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2096c-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="2096c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2096c-116">Application</span></span> | <span data-ttu-id="2096c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2096c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2096c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2096c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}

```
## <a name="request-headers"></a><span data-ttu-id="2096c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2096c-119">Request headers</span></span>
| <span data-ttu-id="2096c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2096c-120">Name</span></span>       | <span data-ttu-id="2096c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2096c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2096c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2096c-122">Authorization</span></span>  | <span data-ttu-id="2096c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2096c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2096c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2096c-125">Request body</span></span>
<span data-ttu-id="2096c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2096c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2096c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="2096c-127">Response</span></span>

<span data-ttu-id="2096c-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2096c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2096c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2096c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2096c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2096c-131">Request</span></span>
<span data-ttu-id="2096c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2096c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskgroups('AAMkADIyAAAhrbe-AAA=')
```
##### <a name="response"></a><span data-ttu-id="2096c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2096c-133">Response</span></span>
<span data-ttu-id="2096c-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2096c-134">Here is an example of the response.</span></span>
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

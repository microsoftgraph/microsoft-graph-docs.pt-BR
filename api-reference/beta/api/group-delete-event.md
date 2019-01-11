---
title: Excluir evento
description: Excluir um objeto event.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: e120910aa35aea0d7b8e74a356204e6aea2509d3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813381"
---
# <a name="delete-event"></a><span data-ttu-id="6585f-103">Excluir evento</span><span class="sxs-lookup"><span data-stu-id="6585f-103">Delete event</span></span>

> <span data-ttu-id="6585f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6585f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6585f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6585f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6585f-106">Excluir um objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="6585f-106">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6585f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6585f-107">Permissions</span></span>
<span data-ttu-id="6585f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6585f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6585f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6585f-110">Permission type</span></span>      | <span data-ttu-id="6585f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6585f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6585f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6585f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6585f-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6585f-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6585f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6585f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6585f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6585f-115">Not supported.</span></span>    |
|<span data-ttu-id="6585f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6585f-116">Application</span></span> | <span data-ttu-id="6585f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6585f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6585f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6585f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6585f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6585f-119">Request headers</span></span>
| <span data-ttu-id="6585f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6585f-120">Name</span></span>       | <span data-ttu-id="6585f-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6585f-121">Type</span></span> | <span data-ttu-id="6585f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6585f-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6585f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6585f-123">Authorization</span></span>  | <span data-ttu-id="6585f-124">string</span><span class="sxs-lookup"><span data-stu-id="6585f-124">string</span></span>  | <span data-ttu-id="6585f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6585f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6585f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6585f-127">Request body</span></span>
<span data-ttu-id="6585f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6585f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6585f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6585f-129">Response</span></span>
<span data-ttu-id="6585f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6585f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6585f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6585f-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6585f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6585f-133">Request</span></span>
<span data-ttu-id="6585f-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6585f-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="6585f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6585f-135">Response</span></span>
<span data-ttu-id="6585f-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6585f-136">The following is an example of the response.</span></span> 
><span data-ttu-id="6585f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6585f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Atualizar evento
description: Atualize um objeto event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 092e5fdb8f70ec73d1c8a33230f596b9fdbf3b19
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979996"
---
# <a name="update-event"></a><span data-ttu-id="d0e58-103">Atualizar evento</span><span class="sxs-lookup"><span data-stu-id="d0e58-103">Update event</span></span>

> <span data-ttu-id="d0e58-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d0e58-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0e58-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d0e58-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0e58-106">Atualize um objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="d0e58-106">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0e58-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0e58-107">Permissions</span></span>
<span data-ttu-id="d0e58-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0e58-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0e58-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0e58-110">Permission type</span></span>      | <span data-ttu-id="d0e58-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0e58-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0e58-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0e58-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d0e58-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0e58-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0e58-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0e58-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0e58-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0e58-115">Not supported.</span></span>    |
|<span data-ttu-id="d0e58-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0e58-116">Application</span></span> | <span data-ttu-id="d0e58-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0e58-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0e58-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0e58-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d0e58-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0e58-119">Request headers</span></span>
| <span data-ttu-id="d0e58-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d0e58-120">Name</span></span>       | <span data-ttu-id="d0e58-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0e58-121">Type</span></span> | <span data-ttu-id="d0e58-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0e58-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d0e58-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0e58-123">Authorization</span></span>  | <span data-ttu-id="d0e58-124">string</span><span class="sxs-lookup"><span data-stu-id="d0e58-124">string</span></span>  | <span data-ttu-id="d0e58-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0e58-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0e58-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0e58-127">Request body</span></span>
<span data-ttu-id="d0e58-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d0e58-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="d0e58-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0e58-131">Response</span></span>
<span data-ttu-id="d0e58-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d0e58-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d0e58-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0e58-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d0e58-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0e58-134">Request</span></span>
<span data-ttu-id="d0e58-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0e58-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/{id}/events/{id}
Content-type: application/json
Content-length: 211

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

#### <a name="response"></a><span data-ttu-id="d0e58-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0e58-136">Response</span></span>
<span data-ttu-id="d0e58-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d0e58-137">The following is an example of the response.</span></span>

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
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

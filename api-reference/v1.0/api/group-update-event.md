---
title: Atualizar evento
description: Atualize um objeto event.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: dd287032c898e4a56983a77815ce12daef05dae9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892264"
---
# <a name="update-event"></a><span data-ttu-id="f945b-103">Atualizar evento</span><span class="sxs-lookup"><span data-stu-id="f945b-103">Update event</span></span>
<span data-ttu-id="f945b-104">Atualize um objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="f945b-104">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f945b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f945b-105">Permissions</span></span>
<span data-ttu-id="f945b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f945b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f945b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f945b-108">Permission type</span></span>      | <span data-ttu-id="f945b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f945b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f945b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f945b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f945b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f945b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f945b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f945b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f945b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f945b-113">Not supported.</span></span>    |
|<span data-ttu-id="f945b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f945b-114">Application</span></span> | <span data-ttu-id="f945b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f945b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f945b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f945b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f945b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f945b-117">Request headers</span></span>
| <span data-ttu-id="f945b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f945b-118">Name</span></span>       | <span data-ttu-id="f945b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f945b-119">Type</span></span> | <span data-ttu-id="f945b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f945b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f945b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f945b-121">Authorization</span></span>  | <span data-ttu-id="f945b-122">string</span><span class="sxs-lookup"><span data-stu-id="f945b-122">string</span></span>  | <span data-ttu-id="f945b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f945b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f945b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f945b-125">Request body</span></span>
<span data-ttu-id="f945b-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f945b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="f945b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f945b-129">Response</span></span>
<span data-ttu-id="f945b-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f945b-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f945b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f945b-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f945b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f945b-132">Request</span></span>
<span data-ttu-id="f945b-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f945b-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/events/{id}
Content-type: application/json
Content-length: 211

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

#### <a name="response"></a><span data-ttu-id="f945b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f945b-134">Response</span></span>
<span data-ttu-id="f945b-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f945b-135">The following is an example of the response.</span></span>

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

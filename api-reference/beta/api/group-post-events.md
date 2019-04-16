---
title: Criar evento
description: Use esta API para criar um novo event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 978f156302380edc05df79ec3a53c1ab0f853f41
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2019
ms.locfileid: "31889951"
---
# <a name="create-event"></a><span data-ttu-id="3f891-103">Criar evento</span><span class="sxs-lookup"><span data-stu-id="3f891-103">Create event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f891-104">Use esta API para criar um novo [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="3f891-104">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3f891-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3f891-105">Permissions</span></span>
<span data-ttu-id="3f891-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f891-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f891-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f891-108">Permission type</span></span>      | <span data-ttu-id="3f891-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3f891-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f891-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f891-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3f891-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f891-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3f891-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f891-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f891-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f891-113">Not supported.</span></span>    |
|<span data-ttu-id="3f891-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f891-114">Application</span></span> | <span data-ttu-id="3f891-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f891-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f891-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f891-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="3f891-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f891-117">Request headers</span></span>
| <span data-ttu-id="3f891-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3f891-118">Header</span></span>       | <span data-ttu-id="3f891-119">Valor</span><span class="sxs-lookup"><span data-stu-id="3f891-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3f891-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f891-120">Authorization</span></span>  | <span data-ttu-id="3f891-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f891-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3f891-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f891-123">Request body</span></span>
<span data-ttu-id="3f891-124">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="3f891-124">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3f891-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f891-125">Response</span></span>
<span data-ttu-id="3f891-126">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f891-126">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f891-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f891-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3f891-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f891-128">Request</span></span>
<span data-ttu-id="3f891-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f891-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="3f891-130">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="3f891-130">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="3f891-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f891-131">Response</span></span>
<span data-ttu-id="3f891-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3f891-132">The following is an example of the response.</span></span>
><span data-ttu-id="3f891-133">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3f891-133">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3f891-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f891-134">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-events.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

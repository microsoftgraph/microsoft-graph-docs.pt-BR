---
title: Criar evento
description: Use esta API para criar um novo event.
author: dkershaw10
ms.openlocfilehash: ab9236df5a359fff7bf4ef669e69336866651516
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331119"
---
# <a name="create-event"></a><span data-ttu-id="b02aa-103">Criar evento</span><span class="sxs-lookup"><span data-stu-id="b02aa-103">Create event</span></span>

> <span data-ttu-id="b02aa-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b02aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b02aa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b02aa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b02aa-106">Use esta API para criar um novo [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="b02aa-106">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b02aa-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b02aa-107">Permissions</span></span>
<span data-ttu-id="b02aa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b02aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b02aa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b02aa-110">Permission type</span></span>      | <span data-ttu-id="b02aa-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b02aa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b02aa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b02aa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b02aa-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b02aa-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b02aa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b02aa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b02aa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b02aa-115">Not supported.</span></span>    |
|<span data-ttu-id="b02aa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b02aa-116">Application</span></span> | <span data-ttu-id="b02aa-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b02aa-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b02aa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b02aa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="b02aa-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b02aa-119">Request headers</span></span>
| <span data-ttu-id="b02aa-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b02aa-120">Header</span></span>       | <span data-ttu-id="b02aa-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b02aa-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b02aa-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b02aa-122">Authorization</span></span>  | <span data-ttu-id="b02aa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b02aa-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b02aa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b02aa-125">Request body</span></span>
<span data-ttu-id="b02aa-126">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="b02aa-126">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b02aa-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b02aa-127">Response</span></span>
<span data-ttu-id="b02aa-128">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b02aa-128">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b02aa-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b02aa-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b02aa-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b02aa-130">Request</span></span>
<span data-ttu-id="b02aa-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b02aa-131">The following is an example of the request.</span></span>
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
<span data-ttu-id="b02aa-132">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="b02aa-132">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="b02aa-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b02aa-133">Response</span></span>
<span data-ttu-id="b02aa-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b02aa-134">The following is an example of the response.</span></span>
><span data-ttu-id="b02aa-135">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b02aa-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b02aa-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b02aa-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

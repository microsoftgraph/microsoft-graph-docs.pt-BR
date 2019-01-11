---
title: Listar eventos
description: Recupere uma lista de objetos de evento.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 32051d6192d9de8e692c063011933a951d4fe4bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809300"
---
# <a name="list-events"></a><span data-ttu-id="9814e-103">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="9814e-103">List events</span></span>

> <span data-ttu-id="9814e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9814e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9814e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9814e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9814e-106">Recupere uma lista de objetos [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="9814e-106">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9814e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9814e-107">Permissions</span></span>
<span data-ttu-id="9814e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9814e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9814e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9814e-110">Permission type</span></span>      | <span data-ttu-id="9814e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9814e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9814e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9814e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9814e-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9814e-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9814e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9814e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9814e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9814e-115">Not supported.</span></span>    |
|<span data-ttu-id="9814e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9814e-116">Application</span></span> | <span data-ttu-id="9814e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9814e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9814e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9814e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9814e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9814e-119">Optional query parameters</span></span>
<span data-ttu-id="9814e-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9814e-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9814e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9814e-121">Request headers</span></span>
| <span data-ttu-id="9814e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9814e-122">Name</span></span>       | <span data-ttu-id="9814e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9814e-123">Type</span></span> | <span data-ttu-id="9814e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9814e-124">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="9814e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9814e-125">Authorization</span></span>  | <span data-ttu-id="9814e-126">string</span><span class="sxs-lookup"><span data-stu-id="9814e-126">string</span></span> | <span data-ttu-id="9814e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9814e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9814e-129">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="9814e-129">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="9814e-130">string</span><span class="sxs-lookup"><span data-stu-id="9814e-130">string</span></span> | <span data-ttu-id="9814e-131">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="9814e-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="9814e-132">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="9814e-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="9814e-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9814e-133">Optional.</span></span> |
| <span data-ttu-id="9814e-134">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="9814e-134">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="9814e-135">string</span><span class="sxs-lookup"><span data-stu-id="9814e-135">string</span></span> | <span data-ttu-id="9814e-136">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="9814e-136">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="9814e-137">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="9814e-137">Values can be "text" or "html".</span></span> <span data-ttu-id="9814e-138">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="9814e-138">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="9814e-139">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="9814e-139">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="9814e-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9814e-140">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9814e-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9814e-141">Request body</span></span>
<span data-ttu-id="9814e-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9814e-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9814e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9814e-143">Response</span></span>
<span data-ttu-id="9814e-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9814e-144">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9814e-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9814e-145">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9814e-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9814e-146">Request</span></span>
<span data-ttu-id="9814e-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9814e-147">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/events
```

#### <a name="response"></a><span data-ttu-id="9814e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="9814e-148">Response</span></span>
<span data-ttu-id="9814e-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9814e-149">The following is an example of the response.</span></span>
><span data-ttu-id="9814e-150">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9814e-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9814e-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9814e-151">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List group events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

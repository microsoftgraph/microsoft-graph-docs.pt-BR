---
title: Listar eventos
description: Recupere uma lista de objetos de evento.
ms.openlocfilehash: bb79676e63cf12731a39dceb94e8a1b8b8cf2247
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036532"
---
# <a name="list-events"></a><span data-ttu-id="1e4ad-103">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="1e4ad-103">List events</span></span>

> <span data-ttu-id="1e4ad-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e4ad-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e4ad-106">Recupere uma lista de objetos [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="1e4ad-106">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e4ad-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e4ad-107">Permissions</span></span>
<span data-ttu-id="1e4ad-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e4ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e4ad-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e4ad-110">Permission type</span></span>      | <span data-ttu-id="1e4ad-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e4ad-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e4ad-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e4ad-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1e4ad-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e4ad-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1e4ad-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e4ad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e4ad-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-115">Not supported.</span></span>    |
|<span data-ttu-id="1e4ad-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e4ad-116">Application</span></span> | <span data-ttu-id="1e4ad-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e4ad-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e4ad-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1e4ad-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1e4ad-119">Optional query parameters</span></span>
<span data-ttu-id="1e4ad-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e4ad-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e4ad-121">Request headers</span></span>
| <span data-ttu-id="1e4ad-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1e4ad-122">Name</span></span>       | <span data-ttu-id="1e4ad-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e4ad-123">Type</span></span> | <span data-ttu-id="1e4ad-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e4ad-124">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="1e4ad-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e4ad-125">Authorization</span></span>  | <span data-ttu-id="1e4ad-126">string</span><span class="sxs-lookup"><span data-stu-id="1e4ad-126">string</span></span> | <span data-ttu-id="1e4ad-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1e4ad-129">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="1e4ad-129">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="1e4ad-130">string</span><span class="sxs-lookup"><span data-stu-id="1e4ad-130">string</span></span> | <span data-ttu-id="1e4ad-131">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="1e4ad-132">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="1e4ad-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-133">Optional.</span></span> |
| <span data-ttu-id="1e4ad-134">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="1e4ad-134">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="1e4ad-135">string</span><span class="sxs-lookup"><span data-stu-id="1e4ad-135">string</span></span> | <span data-ttu-id="1e4ad-136">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-136">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="1e4ad-137">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="1e4ad-137">Values can be "text" or "html".</span></span> <span data-ttu-id="1e4ad-138">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-138">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="1e4ad-139">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-139">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="1e4ad-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-140">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e4ad-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e4ad-141">Request body</span></span>
<span data-ttu-id="1e4ad-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e4ad-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e4ad-143">Response</span></span>
<span data-ttu-id="1e4ad-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-144">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e4ad-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e4ad-145">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1e4ad-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e4ad-146">Request</span></span>
<span data-ttu-id="1e4ad-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-147">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/events
```

#### <a name="response"></a><span data-ttu-id="1e4ad-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e4ad-148">Response</span></span>
<span data-ttu-id="1e4ad-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-149">The following is an example of the response.</span></span>
><span data-ttu-id="1e4ad-150">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1e4ad-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e4ad-151">All the properties will be returned from an actual call.</span></span>
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

---
title: Listar eventos
description: Recuperar uma lista de objetos event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 728aba79d2d6a1f591fba000560553acfb33ae5d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263151"
---
# <a name="list-events"></a><span data-ttu-id="8f161-103">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="8f161-103">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f161-104">Recupere uma lista de objetos [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="8f161-104">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f161-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f161-105">Permissions</span></span>
<span data-ttu-id="8f161-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f161-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f161-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f161-108">Permission type</span></span>      | <span data-ttu-id="8f161-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f161-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f161-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f161-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f161-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f161-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8f161-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f161-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f161-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f161-113">Not supported.</span></span>    |
|<span data-ttu-id="8f161-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f161-114">Application</span></span> | <span data-ttu-id="8f161-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f161-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f161-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f161-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f161-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8f161-117">Optional query parameters</span></span>
<span data-ttu-id="8f161-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8f161-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f161-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f161-119">Request headers</span></span>
| <span data-ttu-id="8f161-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8f161-120">Name</span></span>       | <span data-ttu-id="8f161-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f161-121">Type</span></span> | <span data-ttu-id="8f161-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f161-122">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="8f161-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f161-123">Authorization</span></span>  | <span data-ttu-id="8f161-124">string</span><span class="sxs-lookup"><span data-stu-id="8f161-124">string</span></span> | <span data-ttu-id="8f161-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f161-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8f161-127">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="8f161-127">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="8f161-128">string</span><span class="sxs-lookup"><span data-stu-id="8f161-128">string</span></span> | <span data-ttu-id="8f161-129">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="8f161-129">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="8f161-130">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="8f161-130">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="8f161-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8f161-131">Optional.</span></span> |
| <span data-ttu-id="8f161-132">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="8f161-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="8f161-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f161-133">string</span></span> | <span data-ttu-id="8f161-134">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="8f161-134">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="8f161-135">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="8f161-135">Values can be "text" or "html".</span></span> <span data-ttu-id="8f161-136">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="8f161-136">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="8f161-137">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="8f161-137">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="8f161-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8f161-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f161-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f161-139">Request body</span></span>
<span data-ttu-id="8f161-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8f161-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f161-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f161-141">Response</span></span>
<span data-ttu-id="8f161-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f161-142">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f161-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f161-143">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8f161-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f161-144">Request</span></span>
<span data-ttu-id="8f161-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f161-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/events
```

#### <a name="response"></a><span data-ttu-id="8f161-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f161-146">Response</span></span>
<span data-ttu-id="8f161-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f161-147">The following is an example of the response.</span></span>
><span data-ttu-id="8f161-148">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8f161-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8f161-149">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f161-149">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8f161-150">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="8f161-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8f161-151">C#</span><span class="sxs-lookup"><span data-stu-id="8f161-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_events-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f161-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f161-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_events-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8f161-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8f161-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_group_events-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-events.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-list-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

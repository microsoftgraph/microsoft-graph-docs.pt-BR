---
title: Listar eventos
description: Recuperar uma lista de objetos event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6a8ff2621089214d30b9b7aa8d06c069312f3c6c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419601"
---
# <a name="list-events"></a><span data-ttu-id="1f903-103">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="1f903-103">List events</span></span>

<span data-ttu-id="1f903-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1f903-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f903-105">Recupere uma lista de objetos [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="1f903-105">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f903-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f903-106">Permissions</span></span>
<span data-ttu-id="1f903-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f903-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f903-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f903-109">Permission type</span></span>      | <span data-ttu-id="1f903-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f903-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f903-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f903-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1f903-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f903-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1f903-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f903-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f903-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f903-114">Not supported.</span></span>    |
|<span data-ttu-id="1f903-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f903-115">Application</span></span> | <span data-ttu-id="1f903-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f903-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f903-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f903-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f903-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1f903-118">Optional query parameters</span></span>
<span data-ttu-id="1f903-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1f903-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f903-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f903-120">Request headers</span></span>
| <span data-ttu-id="1f903-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1f903-121">Name</span></span>       | <span data-ttu-id="1f903-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f903-122">Type</span></span> | <span data-ttu-id="1f903-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f903-123">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="1f903-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f903-124">Authorization</span></span>  | <span data-ttu-id="1f903-125">string</span><span class="sxs-lookup"><span data-stu-id="1f903-125">string</span></span> | <span data-ttu-id="1f903-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f903-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1f903-128">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="1f903-128">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="1f903-129">string</span><span class="sxs-lookup"><span data-stu-id="1f903-129">string</span></span> | <span data-ttu-id="1f903-130">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="1f903-130">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="1f903-131">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="1f903-131">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="1f903-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1f903-132">Optional.</span></span> |
| <span data-ttu-id="1f903-133">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="1f903-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="1f903-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f903-134">string</span></span> | <span data-ttu-id="1f903-135">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="1f903-135">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="1f903-136">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="1f903-136">Values can be "text" or "html".</span></span> <span data-ttu-id="1f903-137">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="1f903-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="1f903-138">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="1f903-138">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="1f903-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1f903-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f903-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f903-140">Request body</span></span>
<span data-ttu-id="1f903-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f903-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f903-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f903-142">Response</span></span>
<span data-ttu-id="1f903-143">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f903-143">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f903-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f903-144">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1f903-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f903-145">Request</span></span>
<span data-ttu-id="1f903-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f903-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f903-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f903-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/events
```
# <a name="c"></a>[<span data-ttu-id="1f903-148">C#</span><span class="sxs-lookup"><span data-stu-id="1f903-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f903-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f903-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f903-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f903-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1f903-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f903-151">Response</span></span>
<span data-ttu-id="1f903-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1f903-152">The following is an example of the response.</span></span>
><span data-ttu-id="1f903-p105">**Observação:** o objeto de resposta mostrado aqui pode ser reduzido para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f903-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List group events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

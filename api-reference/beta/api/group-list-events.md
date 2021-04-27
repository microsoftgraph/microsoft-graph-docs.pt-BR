---
title: Listar eventos
description: Recuperar uma lista de objetos event.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: cbdb6eff39e2e7139bf8c78ac739148fb7059794
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041635"
---
# <a name="list-events"></a><span data-ttu-id="762b1-103">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="762b1-103">List events</span></span>

<span data-ttu-id="762b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="762b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="762b1-105">Recupere uma lista de objetos [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="762b1-105">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="762b1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="762b1-106">Permissions</span></span>
<span data-ttu-id="762b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="762b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="762b1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="762b1-109">Permission type</span></span>      | <span data-ttu-id="762b1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="762b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="762b1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="762b1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="762b1-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="762b1-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="762b1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="762b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="762b1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="762b1-114">Not supported.</span></span>    |
|<span data-ttu-id="762b1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="762b1-115">Application</span></span> | <span data-ttu-id="762b1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="762b1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="762b1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="762b1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="762b1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="762b1-118">Optional query parameters</span></span>
<span data-ttu-id="762b1-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="762b1-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="762b1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="762b1-120">Request headers</span></span>
| <span data-ttu-id="762b1-121">Nome</span><span class="sxs-lookup"><span data-stu-id="762b1-121">Name</span></span>       | <span data-ttu-id="762b1-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="762b1-122">Type</span></span> | <span data-ttu-id="762b1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="762b1-123">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="762b1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="762b1-124">Authorization</span></span>  | <span data-ttu-id="762b1-125">string</span><span class="sxs-lookup"><span data-stu-id="762b1-125">string</span></span> | <span data-ttu-id="762b1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="762b1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="762b1-128">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="762b1-128">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="762b1-129">string</span><span class="sxs-lookup"><span data-stu-id="762b1-129">string</span></span> | <span data-ttu-id="762b1-130">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="762b1-130">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="762b1-131">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="762b1-131">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="762b1-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="762b1-132">Optional.</span></span> |
| <span data-ttu-id="762b1-133">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="762b1-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="762b1-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="762b1-134">string</span></span> | <span data-ttu-id="762b1-135">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="762b1-135">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="762b1-136">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="762b1-136">Values can be "text" or "html".</span></span> <span data-ttu-id="762b1-137">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="762b1-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="762b1-138">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="762b1-138">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="762b1-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="762b1-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="762b1-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="762b1-140">Request body</span></span>
<span data-ttu-id="762b1-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="762b1-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="762b1-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="762b1-142">Response</span></span>
<span data-ttu-id="762b1-143">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="762b1-143">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="762b1-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="762b1-144">Example</span></span>
#### <a name="request"></a><span data-ttu-id="762b1-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="762b1-145">Request</span></span>
<span data-ttu-id="762b1-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="762b1-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="762b1-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="762b1-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/events
```
# <a name="c"></a>[<span data-ttu-id="762b1-148">C#</span><span class="sxs-lookup"><span data-stu-id="762b1-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="762b1-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="762b1-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="762b1-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="762b1-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="762b1-151">Java</span><span class="sxs-lookup"><span data-stu-id="762b1-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="762b1-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="762b1-152">Response</span></span>
<span data-ttu-id="762b1-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="762b1-153">The following is an example of the response.</span></span>
><span data-ttu-id="762b1-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="762b1-154">**Note:** The response object shown here might be shortened for readability.</span></span>
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



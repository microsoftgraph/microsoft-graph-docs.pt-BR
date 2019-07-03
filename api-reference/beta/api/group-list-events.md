---
title: Listar eventos
description: Recuperar uma lista de objetos event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 6c25596349c5475368188f7ed36be0d74120a4de
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440453"
---
# <a name="list-events"></a><span data-ttu-id="72711-103">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="72711-103">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72711-104">Recupere uma lista de objetos [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="72711-104">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="72711-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="72711-105">Permissions</span></span>
<span data-ttu-id="72711-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72711-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72711-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72711-108">Permission type</span></span>      | <span data-ttu-id="72711-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72711-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72711-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72711-110">Delegated (work or school account)</span></span> | <span data-ttu-id="72711-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72711-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="72711-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72711-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72711-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72711-113">Not supported.</span></span>    |
|<span data-ttu-id="72711-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72711-114">Application</span></span> | <span data-ttu-id="72711-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72711-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72711-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72711-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72711-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="72711-117">Optional query parameters</span></span>
<span data-ttu-id="72711-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="72711-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72711-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72711-119">Request headers</span></span>
| <span data-ttu-id="72711-120">Nome</span><span class="sxs-lookup"><span data-stu-id="72711-120">Name</span></span>       | <span data-ttu-id="72711-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="72711-121">Type</span></span> | <span data-ttu-id="72711-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="72711-122">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="72711-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="72711-123">Authorization</span></span>  | <span data-ttu-id="72711-124">string</span><span class="sxs-lookup"><span data-stu-id="72711-124">string</span></span> | <span data-ttu-id="72711-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72711-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="72711-127">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="72711-127">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="72711-128">string</span><span class="sxs-lookup"><span data-stu-id="72711-128">string</span></span> | <span data-ttu-id="72711-129">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="72711-129">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="72711-130">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="72711-130">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="72711-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="72711-131">Optional.</span></span> |
| <span data-ttu-id="72711-132">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="72711-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="72711-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72711-133">string</span></span> | <span data-ttu-id="72711-134">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="72711-134">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="72711-135">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="72711-135">Values can be "text" or "html".</span></span> <span data-ttu-id="72711-136">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="72711-136">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="72711-137">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="72711-137">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="72711-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="72711-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72711-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72711-139">Request body</span></span>
<span data-ttu-id="72711-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72711-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72711-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="72711-141">Response</span></span>
<span data-ttu-id="72711-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72711-142">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72711-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72711-143">Example</span></span>
#### <a name="request"></a><span data-ttu-id="72711-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72711-144">Request</span></span>
<span data-ttu-id="72711-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="72711-145">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="72711-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="72711-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/events
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="72711-147">C#</span><span class="sxs-lookup"><span data-stu-id="72711-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72711-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="72711-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="72711-149">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="72711-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="72711-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="72711-150">Response</span></span>
<span data-ttu-id="72711-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="72711-151">The following is an example of the response.</span></span>
><span data-ttu-id="72711-152">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="72711-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="72711-153">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72711-153">All the properties will be returned from an actual call.</span></span>
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

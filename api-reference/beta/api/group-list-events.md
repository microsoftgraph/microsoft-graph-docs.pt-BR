---
title: Listar eventos
description: Recupere uma lista de objetos de evento.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c02318a8c7a8c7a8ffc7562d4a807fa06fae47a6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525378"
---
# <a name="list-events"></a><span data-ttu-id="85b70-103">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="85b70-103">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85b70-104">Recupere uma lista de objetos [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="85b70-104">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="85b70-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="85b70-105">Permissions</span></span>
<span data-ttu-id="85b70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85b70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85b70-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85b70-108">Permission type</span></span>      | <span data-ttu-id="85b70-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85b70-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85b70-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85b70-110">Delegated (work or school account)</span></span> | <span data-ttu-id="85b70-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85b70-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="85b70-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85b70-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85b70-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85b70-113">Not supported.</span></span>    |
|<span data-ttu-id="85b70-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85b70-114">Application</span></span> | <span data-ttu-id="85b70-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85b70-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85b70-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85b70-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="85b70-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="85b70-117">Optional query parameters</span></span>
<span data-ttu-id="85b70-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="85b70-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85b70-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85b70-119">Request headers</span></span>
| <span data-ttu-id="85b70-120">Nome</span><span class="sxs-lookup"><span data-stu-id="85b70-120">Name</span></span>       | <span data-ttu-id="85b70-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="85b70-121">Type</span></span> | <span data-ttu-id="85b70-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="85b70-122">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="85b70-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="85b70-123">Authorization</span></span>  | <span data-ttu-id="85b70-124">string</span><span class="sxs-lookup"><span data-stu-id="85b70-124">string</span></span> | <span data-ttu-id="85b70-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85b70-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="85b70-127">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="85b70-127">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="85b70-128">string</span><span class="sxs-lookup"><span data-stu-id="85b70-128">string</span></span> | <span data-ttu-id="85b70-129">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="85b70-129">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="85b70-130">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="85b70-130">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="85b70-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="85b70-131">Optional.</span></span> |
| <span data-ttu-id="85b70-132">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="85b70-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="85b70-133">string</span><span class="sxs-lookup"><span data-stu-id="85b70-133">string</span></span> | <span data-ttu-id="85b70-134">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="85b70-134">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="85b70-135">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="85b70-135">Values can be "text" or "html".</span></span> <span data-ttu-id="85b70-136">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="85b70-136">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="85b70-137">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="85b70-137">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="85b70-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="85b70-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85b70-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85b70-139">Request body</span></span>
<span data-ttu-id="85b70-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85b70-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85b70-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="85b70-141">Response</span></span>
<span data-ttu-id="85b70-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85b70-142">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85b70-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85b70-143">Example</span></span>
#### <a name="request"></a><span data-ttu-id="85b70-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85b70-144">Request</span></span>
<span data-ttu-id="85b70-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="85b70-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/events
```

#### <a name="response"></a><span data-ttu-id="85b70-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="85b70-146">Response</span></span>
<span data-ttu-id="85b70-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="85b70-147">The following is an example of the response.</span></span>
><span data-ttu-id="85b70-148">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="85b70-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="85b70-149">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85b70-149">All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/group-list-events.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

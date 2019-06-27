---
title: Listar timesOff
description: Obtenha a lista de timesOff neste cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d35d5b1428fd54f2837c34bfe4a8f90aeff58b1f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264033"
---
# <a name="list-timesoff"></a><span data-ttu-id="446f7-103">Listar timesOff</span><span class="sxs-lookup"><span data-stu-id="446f7-103">List timesOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="446f7-104">Obtenha a lista de instâncias do [timeOff](../resources/timeoff.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="446f7-104">Get the list of [timeOff](../resources/timeoff.md) instances in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="446f7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="446f7-105">Permissions</span></span>

<span data-ttu-id="446f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="446f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="446f7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="446f7-108">Permission type</span></span>      | <span data-ttu-id="446f7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="446f7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="446f7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="446f7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="446f7-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="446f7-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="446f7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="446f7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="446f7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="446f7-113">Not supported.</span></span>    |
|<span data-ttu-id="446f7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="446f7-114">Application</span></span> | <span data-ttu-id="446f7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="446f7-115">Not supported.</span></span> |

> <span data-ttu-id="446f7-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="446f7-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="446f7-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="446f7-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="446f7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="446f7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff
```
## <a name="optional-query-parameters"></a><span data-ttu-id="446f7-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="446f7-119">Optional query parameters</span></span>
<span data-ttu-id="446f7-120">Este método dá suporte ao [parâmetro de consulta OData](/graph/query-parameters) $Filter para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="446f7-120">This method supports the $filter [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="446f7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="446f7-121">Request headers</span></span>

| <span data-ttu-id="446f7-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="446f7-122">Header</span></span>       | <span data-ttu-id="446f7-123">Valor</span><span class="sxs-lookup"><span data-stu-id="446f7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="446f7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="446f7-124">Authorization</span></span>  | <span data-ttu-id="446f7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="446f7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="446f7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="446f7-127">Content-Type</span></span>  | <span data-ttu-id="446f7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="446f7-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="446f7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="446f7-129">Request body</span></span>
<span data-ttu-id="446f7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="446f7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="446f7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="446f7-131">Response</span></span>

<span data-ttu-id="446f7-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [timeOff](../resources/timeoff.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="446f7-132">If successful, this method returns a `200 OK` response code and a collection of [timeOff](../resources/timeoff.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="446f7-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="446f7-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="446f7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="446f7-134">Request</span></span>

<span data-ttu-id="446f7-135">Veja a seguir um exemplo de uma solicitação que obtém todos os objetos **timeOff** que têm uma versão compartilhada e uma versão de rascunho entre 11 de março de 18 de março de 2019.</span><span class="sxs-lookup"><span data-stu-id="446f7-135">The following is an example of a request that gets all **timeOff** objects that have a shared version and a draft version between March 11 - March 18, 2019.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-list-timesoff"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff?$filter=sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z
```

#### <a name="response"></a><span data-ttu-id="446f7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="446f7-136">Response</span></span>

<span data-ttu-id="446f7-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="446f7-137">The following is an example of the response.</span></span> 

><span data-ttu-id="446f7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="446f7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOff",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
    {
      "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
      "createdDateTime": "2019-03-14T05:35:57.755Z",
      "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
      "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
          "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
          "displayName": "John Doe"
        }
      },
      "sharedTimeOff": {
        "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
        "startDateTime": "2019-03-11T07:00:00Z",
        "endDateTime": "2019-03-12T07:00:00Z",
        "theme": "white"
      },
      "draftTimeOff": {
        "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
        "startDateTime": "2019-03-11T07:00:00Z",
        "endDateTime": "2019-03-12T07:00:00Z",
        "theme": "pink"
      }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="446f7-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="446f7-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="446f7-141">C#</span><span class="sxs-lookup"><span data-stu-id="446f7-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/schedule-list-timesoff-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="446f7-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="446f7-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/schedule-list-timesoff-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="446f7-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="446f7-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/schedule-list-timesoff-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of timesOff in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-list-timesoff.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/schedule-list-timesoff.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schedule-list-timesoff.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

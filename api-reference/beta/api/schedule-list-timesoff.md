---
title: Listar timesOff
description: Obtenha a lista de timesOff neste cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f1f91490eb08d6ebebbed7187c3c4bf5bb05df0f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450349"
---
# <a name="list-timesoff"></a><span data-ttu-id="9bfd2-103">Listar timesOff</span><span class="sxs-lookup"><span data-stu-id="9bfd2-103">List timesOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bfd2-104">Obtenha a lista de instâncias do [timeOff](../resources/timeoff.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="9bfd2-104">Get the list of [timeOff](../resources/timeoff.md) instances in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9bfd2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9bfd2-105">Permissions</span></span>

<span data-ttu-id="9bfd2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bfd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bfd2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bfd2-108">Permission type</span></span>      | <span data-ttu-id="9bfd2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9bfd2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bfd2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bfd2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9bfd2-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bfd2-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9bfd2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bfd2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bfd2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bfd2-113">Not supported.</span></span>    |
|<span data-ttu-id="9bfd2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bfd2-114">Application</span></span> | <span data-ttu-id="9bfd2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bfd2-115">Not supported.</span></span> |

> <span data-ttu-id="9bfd2-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="9bfd2-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9bfd2-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="9bfd2-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9bfd2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bfd2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9bfd2-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9bfd2-119">Optional query parameters</span></span>
<span data-ttu-id="9bfd2-120">Este método dá suporte ao [parâmetro de consulta OData](/graph/query-parameters) $Filter para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9bfd2-120">This method supports the $filter [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bfd2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bfd2-121">Request headers</span></span>

| <span data-ttu-id="9bfd2-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9bfd2-122">Header</span></span>       | <span data-ttu-id="9bfd2-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9bfd2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9bfd2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bfd2-124">Authorization</span></span>  | <span data-ttu-id="9bfd2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bfd2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9bfd2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9bfd2-127">Content-Type</span></span>  | <span data-ttu-id="9bfd2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9bfd2-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9bfd2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bfd2-129">Request body</span></span>
<span data-ttu-id="9bfd2-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9bfd2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bfd2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bfd2-131">Response</span></span>

<span data-ttu-id="9bfd2-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [timeOff](../resources/timeoff.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bfd2-132">If successful, this method returns a `200 OK` response code and a collection of [timeOff](../resources/timeoff.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bfd2-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bfd2-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9bfd2-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bfd2-134">Request</span></span>

<span data-ttu-id="9bfd2-135">Veja a seguir um exemplo de uma solicitação que obtém todos os objetos **timeOff** que têm uma versão compartilhada e uma versão de rascunho entre 11 de março de 18 de março de 2019.</span><span class="sxs-lookup"><span data-stu-id="9bfd2-135">The following is an example of a request that gets all **timeOff** objects that have a shared version and a draft version between March 11 - March 18, 2019.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9bfd2-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bfd2-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-timesoff"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff?$filter=sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9bfd2-137">C#</span><span class="sxs-lookup"><span data-stu-id="9bfd2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-timesoff-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9bfd2-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="9bfd2-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-timesoff-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9bfd2-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9bfd2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-timesoff-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9bfd2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bfd2-140">Response</span></span>

<span data-ttu-id="9bfd2-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9bfd2-141">The following is an example of the response.</span></span> 

><span data-ttu-id="9bfd2-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9bfd2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->

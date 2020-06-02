---
title: Listar timesOff
description: Obtenha a lista de timesOff neste cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a1f3ad2ca2ad07e6285337513dfa7cf5ee151a13
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "42453839"
---
# <a name="list-timesoff"></a><span data-ttu-id="949d2-103">Listar timesOff</span><span class="sxs-lookup"><span data-stu-id="949d2-103">List timesOff</span></span>

<span data-ttu-id="949d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="949d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="949d2-105">Obtenha a lista de instâncias do [timeOff](../resources/timeoff.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="949d2-105">Get the list of [timeOff](../resources/timeoff.md) instances in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="949d2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="949d2-106">Permissions</span></span>

<span data-ttu-id="949d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="949d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="949d2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="949d2-109">Permission type</span></span>      | <span data-ttu-id="949d2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="949d2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="949d2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="949d2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="949d2-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="949d2-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="949d2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="949d2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="949d2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="949d2-114">Not supported.</span></span>    |
|<span data-ttu-id="949d2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="949d2-115">Application</span></span> | <span data-ttu-id="949d2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="949d2-116">Not supported.</span></span> |

> <span data-ttu-id="949d2-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="949d2-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="949d2-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="949d2-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="949d2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="949d2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff
```
## <a name="optional-query-parameters"></a><span data-ttu-id="949d2-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="949d2-120">Optional query parameters</span></span>
<span data-ttu-id="949d2-121">Este método dá suporte ao [parâmetro de consulta OData](/graph/query-parameters) $Filter para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="949d2-121">This method supports the $filter [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="949d2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="949d2-122">Request headers</span></span>

| <span data-ttu-id="949d2-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="949d2-123">Header</span></span>       | <span data-ttu-id="949d2-124">Valor</span><span class="sxs-lookup"><span data-stu-id="949d2-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="949d2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="949d2-125">Authorization</span></span>  | <span data-ttu-id="949d2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="949d2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="949d2-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="949d2-128">Content-Type</span></span>  | <span data-ttu-id="949d2-129">application/json</span><span class="sxs-lookup"><span data-stu-id="949d2-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="949d2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="949d2-130">Request body</span></span>
<span data-ttu-id="949d2-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="949d2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="949d2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="949d2-132">Response</span></span>

<span data-ttu-id="949d2-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [timeOff](../resources/timeoff.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="949d2-133">If successful, this method returns a `200 OK` response code and a collection of [timeOff](../resources/timeoff.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="949d2-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="949d2-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="949d2-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="949d2-135">Request</span></span>

<span data-ttu-id="949d2-136">Veja a seguir um exemplo de uma solicitação que obtém todos os objetos **timeOff** que têm uma versão compartilhada e uma versão de rascunho entre 11 de março de 18 de março de 2019.</span><span class="sxs-lookup"><span data-stu-id="949d2-136">The following is an example of a request that gets all **timeOff** objects that have a shared version and a draft version between March 11 - March 18, 2019.</span></span>

# <a name="http"></a>[<span data-ttu-id="949d2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="949d2-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-timesoff"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff?$filter=sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z
```
# <a name="c"></a>[<span data-ttu-id="949d2-138">C#</span><span class="sxs-lookup"><span data-stu-id="949d2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-timesoff-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="949d2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="949d2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-timesoff-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="949d2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="949d2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-timesoff-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="949d2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="949d2-141">Response</span></span>

<span data-ttu-id="949d2-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="949d2-142">The following is an example of the response.</span></span> 

><span data-ttu-id="949d2-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="949d2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

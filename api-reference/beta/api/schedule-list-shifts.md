---
title: Listar turnos
description: Obter a lista de turnos em um cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0565f3e0d5e81bf7bc8cc3c9f153935a01bf90e6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050882"
---
# <a name="list-shifts"></a><span data-ttu-id="f2da8-103">Listar turnos</span><span class="sxs-lookup"><span data-stu-id="f2da8-103">List shifts</span></span>

<span data-ttu-id="f2da8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2da8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="f2da8-105">Obter a lista de [instâncias de turno](../resources/shift.md) em um [agendamento](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="f2da8-105">Get the list of [shift](../resources/shift.md) instances in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2da8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2da8-106">Permissions</span></span>

<span data-ttu-id="f2da8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2da8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2da8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2da8-109">Permission type</span></span>      | <span data-ttu-id="f2da8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2da8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2da8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2da8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f2da8-112">Schedule.Read.All, Group.Read.All,Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2da8-112">Schedule.Read.All, Group.Read.All,Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f2da8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2da8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2da8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2da8-114">Not supported.</span></span>    |
|<span data-ttu-id="f2da8-115">Application</span><span class="sxs-lookup"><span data-stu-id="f2da8-115">Application</span></span> | <span data-ttu-id="f2da8-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2da8-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2da8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2da8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2da8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f2da8-118">Optional query parameters</span></span>
<span data-ttu-id="f2da8-119">Este método dá suporte ao parâmetro $filter [consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f2da8-119">This method supports the $filter [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2da8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2da8-120">Request headers</span></span>

| <span data-ttu-id="f2da8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2da8-121">Header</span></span>       | <span data-ttu-id="f2da8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f2da8-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f2da8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2da8-123">Authorization</span></span>  | <span data-ttu-id="f2da8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2da8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f2da8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2da8-126">Request body</span></span>
<span data-ttu-id="f2da8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2da8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2da8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2da8-128">Response</span></span>

<span data-ttu-id="f2da8-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2da8-129">If successful, this method returns a `200 OK` response code and a collection of [shift](../resources/shift.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2da8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2da8-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f2da8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2da8-131">Request</span></span>

<span data-ttu-id="f2da8-132">A seguir, um exemplo de uma solicitação que obtém todos os objetos **shift** que tenham uma versão compartilhada e uma versão de rascunho entre 11 de março e 18 de março de 2019.</span><span class="sxs-lookup"><span data-stu-id="f2da8-132">The following is an example of a request that gets all **shift** objects that have a shared version and a draft version between March 11 - March 18, 2019.</span></span>

# <a name="http"></a>[<span data-ttu-id="f2da8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2da8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-shifts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts?$filter=sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z
```
# <a name="c"></a>[<span data-ttu-id="f2da8-134">C#</span><span class="sxs-lookup"><span data-stu-id="f2da8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-shifts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2da8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2da8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-shifts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2da8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2da8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-shifts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2da8-137">Java</span><span class="sxs-lookup"><span data-stu-id="f2da8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-list-shifts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f2da8-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2da8-138">Response</span></span>

<span data-ttu-id="f2da8-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f2da8-139">The following is an example of the response.</span></span> 

><span data-ttu-id="f2da8-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f2da8-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
    {
      "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
      "createdDateTime": "2019-03-14T04:32:51.451Z",
      "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
      "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
      "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
      "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
          "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
          "displayName": "John Doe"
        }
      },
      "sharedShift": {
        "displayName": "Day shift",
        "notes": "Please do inventory as part of your shift.",
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-12T00:00:00Z",
        "theme": "blue",
        "activities": [
          {
            "isPaid": true,
            "startDateTime": "2019-03-11T15:00:00Z",
            "endDateTime": "2019-03-11T15:15:00Z",
            "code": "",
            "displayName": "Lunch"
          }
        ]
      },
      "draftShift": {
        "displayName": "Day shift",
        "notes": "Please do inventory as part of your shift.",
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-12T00:00:00Z",
        "theme": "blue",
        "activities": [
          {
            "isPaid": true,
            "startDateTime": "2019-03-11T15:00:00Z",
            "endDateTime": "2019-03-11T15:30:00Z",
            "code": "",
            "displayName": "Lunch"
          }
        ]
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
  "description": "Get the list of shifts in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



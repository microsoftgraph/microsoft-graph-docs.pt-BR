---
title: Criar ou substituir agendamento
description: Criar ou substituir um objeto **Schedule** .
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fa7deb3a8b3ddd4da5ba99d97c270d6ef3b04556
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971071"
---
# <a name="create-or-replace-schedule"></a><span data-ttu-id="56586-103">Criar ou substituir agendamento</span><span class="sxs-lookup"><span data-stu-id="56586-103">Create or replace schedule</span></span>

<span data-ttu-id="56586-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56586-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56586-105">Criar ou substituir um objeto [Schedule](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="56586-105">Create or replace a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="56586-106">O processo de criação de agendamento está em conformidade com a [diretriz de uma API para operações de longa duração com base em recursos (relo)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span><span class="sxs-lookup"><span data-stu-id="56586-106">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="56586-107">Quando os clientes usam o método PUT, se a agenda for provisionada, a operação substituirá a agenda; caso contrário, a operação iniciará o processo de provisionamento de agendamento em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="56586-107">When clients use the PUT method, if the schedule is provisioned, the operation replaces the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="56586-108">Durante o provisionamento de agendamento, os clientes podem usar o [método Get](schedule-get.md) para obter o agendamento e observar a `provisionStatus` propriedade para o estado atual do provisionamento.</span><span class="sxs-lookup"><span data-stu-id="56586-108">During schedule provisioning, clients can use the [GET method](schedule-get.md) to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="56586-109">Se o provisionamento falhar, os clientes poderão obter informações adicionais da `provisionStatusCode` propriedade.</span><span class="sxs-lookup"><span data-stu-id="56586-109">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="56586-110">Os clientes também podem inspecionar a configuração do cronograma.</span><span class="sxs-lookup"><span data-stu-id="56586-110">Clients can also inspect the configuration of the schedule.</span></span>


## <a name="permissions"></a><span data-ttu-id="56586-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="56586-111">Permissions</span></span>

<span data-ttu-id="56586-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56586-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56586-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56586-114">Permission type</span></span>      | <span data-ttu-id="56586-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56586-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56586-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56586-116">Delegated (work or school account)</span></span> | <span data-ttu-id="56586-117">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="56586-117">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="56586-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56586-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56586-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56586-119">Not supported.</span></span>    |
|<span data-ttu-id="56586-120">Application</span><span class="sxs-lookup"><span data-stu-id="56586-120">Application</span></span> | <span data-ttu-id="56586-121">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56586-121">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56586-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56586-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="56586-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56586-123">Request headers</span></span>

| <span data-ttu-id="56586-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56586-124">Header</span></span>       | <span data-ttu-id="56586-125">Valor</span><span class="sxs-lookup"><span data-stu-id="56586-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="56586-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="56586-126">Authorization</span></span>  | <span data-ttu-id="56586-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56586-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="56586-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56586-129">Content-Type</span></span>  | <span data-ttu-id="56586-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56586-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="56586-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56586-132">Request body</span></span>

<span data-ttu-id="56586-133">No corpo da solicitação, forneça uma representação JSON de um objeto [Schedule](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="56586-133">In the request body, supply a JSON representation of a [schedule](../resources/schedule.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="56586-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="56586-134">Response</span></span>

<span data-ttu-id="56586-135">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Schedule](../resources/schedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56586-135">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56586-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56586-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="56586-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56586-137">Request</span></span>

<span data-ttu-id="56586-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="56586-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="56586-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="56586-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team-put-schedule"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule
Content-type: application/json

{
  "enabled": true,
  "timeZone": "America/Chicago"
}
```
# <a name="c"></a>[<span data-ttu-id="56586-140">C#</span><span class="sxs-lookup"><span data-stu-id="56586-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-put-schedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56586-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56586-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-put-schedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56586-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56586-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-put-schedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56586-143">Java</span><span class="sxs-lookup"><span data-stu-id="56586-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-put-schedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="56586-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="56586-144">Response</span></span>

<span data-ttu-id="56586-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="56586-145">The following is an example of the response.</span></span> 

><span data-ttu-id="56586-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56586-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedule"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null,
  "timeClockEnabled": true,
  "openShiftsEnabled": true,
  "swapShiftsRequestsEnabled": true,
  "offerShiftRequestsEnabled": true,
  "timeOffRequestsEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates or replaces the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



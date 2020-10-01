---
title: Criar ou substituir agendamento
description: Criar ou substituir um objeto **Schedule** .
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 51b7a8afbf70899c7f217cb0b0b648ca8f4e7761
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314948"
---
# <a name="create-or-replace-schedule"></a><span data-ttu-id="ed4aa-103">Criar ou substituir agendamento</span><span class="sxs-lookup"><span data-stu-id="ed4aa-103">Create or replace schedule</span></span>

<span data-ttu-id="ed4aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed4aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed4aa-105">Criar ou substituir um objeto [Schedule](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="ed4aa-105">Create or replace a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="ed4aa-106">O processo de criação de agendamento está em conformidade com a [diretriz de uma API para operações de longa duração com base em recursos (relo)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span><span class="sxs-lookup"><span data-stu-id="ed4aa-106">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="ed4aa-107">Quando os clientes usam o método PUT, se a agenda for provisionada, a operação substituirá a agenda; caso contrário, a operação iniciará o processo de provisionamento de agendamento em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="ed4aa-107">When clients use the PUT method, if the schedule is provisioned, the operation replaces the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="ed4aa-108">Durante o provisionamento de agendamento, os clientes podem usar o [método Get](schedule-get.md) para obter o agendamento e observar a `provisionStatus` propriedade para o estado atual do provisionamento.</span><span class="sxs-lookup"><span data-stu-id="ed4aa-108">During schedule provisioning, clients can use the [GET method](schedule-get.md) to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="ed4aa-109">Se o provisionamento falhar, os clientes poderão obter informações adicionais da `provisionStatusCode` propriedade.</span><span class="sxs-lookup"><span data-stu-id="ed4aa-109">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="ed4aa-110">Os clientes também podem inspecionar a configuração do cronograma.</span><span class="sxs-lookup"><span data-stu-id="ed4aa-110">Clients can also inspect the configuration of the schedule.</span></span>


## <a name="permissions"></a><span data-ttu-id="ed4aa-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed4aa-111">Permissions</span></span>

<span data-ttu-id="ed4aa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed4aa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed4aa-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed4aa-114">Permission type</span></span>      | <span data-ttu-id="ed4aa-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed4aa-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed4aa-116">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed4aa-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ed4aa-117">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ed4aa-117">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ed4aa-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed4aa-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed4aa-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed4aa-119">Not supported.</span></span>    |
|<span data-ttu-id="ed4aa-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed4aa-120">Application</span></span> | <span data-ttu-id="ed4aa-121">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed4aa-121">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed4aa-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed4aa-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="ed4aa-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed4aa-123">Request headers</span></span>

| <span data-ttu-id="ed4aa-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed4aa-124">Header</span></span>       | <span data-ttu-id="ed4aa-125">Valor</span><span class="sxs-lookup"><span data-stu-id="ed4aa-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ed4aa-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed4aa-126">Authorization</span></span>  | <span data-ttu-id="ed4aa-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed4aa-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ed4aa-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed4aa-129">Content-Type</span></span>  | <span data-ttu-id="ed4aa-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed4aa-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ed4aa-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed4aa-132">Request body</span></span>

<span data-ttu-id="ed4aa-133">No corpo da solicitação, forneça uma representação JSON de um objeto [Schedule](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="ed4aa-133">In the request body, supply a JSON representation of a [schedule](../resources/schedule.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ed4aa-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed4aa-134">Response</span></span>

<span data-ttu-id="ed4aa-135">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Schedule](../resources/schedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed4aa-135">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed4aa-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed4aa-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed4aa-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed4aa-137">Request</span></span>

<span data-ttu-id="ed4aa-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed4aa-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "team-put-schedule"
}-->
```http
PUT https://graph.microsoft.com/v1/teams/{teamId}/schedule
Content-type: application/json

{
  "enabled": true,
  "timeZone": "America/Chicago"
}
```
---


### <a name="response"></a><span data-ttu-id="ed4aa-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed4aa-139">Response</span></span>

<span data-ttu-id="ed4aa-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ed4aa-140">The following is an example of the response.</span></span> 

><span data-ttu-id="ed4aa-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed4aa-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


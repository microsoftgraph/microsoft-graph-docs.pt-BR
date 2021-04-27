---
title: Obter agendamento
description: Recupere as propriedades e as relações de um **objeto schedule.**
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e0bcc91939ac53adbefe16a97986239fec955ab3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049034"
---
# <a name="get-schedule"></a><span data-ttu-id="28cbf-103">Obter agendamento</span><span class="sxs-lookup"><span data-stu-id="28cbf-103">Get schedule</span></span>

<span data-ttu-id="28cbf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28cbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28cbf-105">Recupere as propriedades e as relações de um [objeto schedule.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="28cbf-105">Retrieve the properties and relationships of a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="28cbf-106">O processo de criação de agendamento está em conformidade com a diretriz da API One para operações de longa execução [(RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo)baseadas em recursos.</span><span class="sxs-lookup"><span data-stu-id="28cbf-106">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="28cbf-107">Quando os clientes usam o [método PUT](team-put-schedule.md), se o agendamento for provisionado, a operação atualiza o cronograma; caso contrário, a operação inicia o processo de provisionamento de agendamento em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="28cbf-107">When clients use the [PUT method](team-put-schedule.md), if the schedule is provisioned, the operation updates the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="28cbf-108">Durante o provisionamento de agendamento, os clientes podem usar o método GET para obter o agendamento e olhar para a propriedade para o estado `provisionStatus` atual do provisionamento.</span><span class="sxs-lookup"><span data-stu-id="28cbf-108">During schedule provisioning, clients can use the GET method to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="28cbf-109">Se o provisionamento falhar, os clientes poderão obter informações adicionais da `provisionStatusCode` propriedade.</span><span class="sxs-lookup"><span data-stu-id="28cbf-109">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="28cbf-110">Os clientes também podem inspecionar a configuração da agenda.</span><span class="sxs-lookup"><span data-stu-id="28cbf-110">Clients can also inspect the configuration of the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="28cbf-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="28cbf-111">Permissions</span></span>

<span data-ttu-id="28cbf-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28cbf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28cbf-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28cbf-114">Permission type</span></span>      | <span data-ttu-id="28cbf-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28cbf-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28cbf-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28cbf-116">Delegated (work or school account)</span></span> | <span data-ttu-id="28cbf-117">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28cbf-117">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="28cbf-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28cbf-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28cbf-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28cbf-119">Not supported.</span></span>    |
|<span data-ttu-id="28cbf-120">Application</span><span class="sxs-lookup"><span data-stu-id="28cbf-120">Application</span></span> | <span data-ttu-id="28cbf-121">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28cbf-121">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="28cbf-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28cbf-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28cbf-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="28cbf-123">Optional query parameters</span></span>

<span data-ttu-id="28cbf-124">Este método não dá suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="28cbf-124">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28cbf-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28cbf-125">Request headers</span></span>

| <span data-ttu-id="28cbf-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28cbf-126">Header</span></span>       | <span data-ttu-id="28cbf-127">Valor</span><span class="sxs-lookup"><span data-stu-id="28cbf-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="28cbf-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="28cbf-128">Authorization</span></span>  | <span data-ttu-id="28cbf-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28cbf-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="28cbf-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28cbf-131">Content-Type</span></span>  | <span data-ttu-id="28cbf-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28cbf-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="28cbf-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28cbf-134">Request body</span></span>
<span data-ttu-id="28cbf-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28cbf-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28cbf-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="28cbf-136">Response</span></span>

<span data-ttu-id="28cbf-137">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [schedule](../resources/schedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28cbf-137">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28cbf-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28cbf-138">Example</span></span>

#### <a name="request"></a><span data-ttu-id="28cbf-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28cbf-139">Request</span></span>

<span data-ttu-id="28cbf-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="28cbf-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28cbf-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="28cbf-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule
```
# <a name="c"></a>[<span data-ttu-id="28cbf-142">C#</span><span class="sxs-lookup"><span data-stu-id="28cbf-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28cbf-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28cbf-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28cbf-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28cbf-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28cbf-145">Java</span><span class="sxs-lookup"><span data-stu-id="28cbf-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="28cbf-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="28cbf-146">Response</span></span>

<span data-ttu-id="28cbf-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="28cbf-147">The following is an example of the response.</span></span> 

><span data-ttu-id="28cbf-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="28cbf-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Get the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



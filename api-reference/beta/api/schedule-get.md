---
title: Obter cronograma
description: Recupere as propriedades e os relacionamentos de um objeto **Schedule** .
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 705c42339dc64ff66f89ce72715d51a6753357d0
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44154245"
---
# <a name="get-schedule"></a><span data-ttu-id="28d5c-103">Obter cronograma</span><span class="sxs-lookup"><span data-stu-id="28d5c-103">Get schedule</span></span>

<span data-ttu-id="28d5c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28d5c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28d5c-105">Recupere as propriedades e os relacionamentos de um objeto [Schedule](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="28d5c-105">Retrieve the properties and relationships of a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="28d5c-106">O processo de criação de agendamento está em conformidade com a [diretriz de uma API para operações de longa duração com base em recursos (relo)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span><span class="sxs-lookup"><span data-stu-id="28d5c-106">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="28d5c-107">Quando os clientes usam o [método Put](team-put-schedule.md), se a agenda for provisionada, a operação atualizará a agenda; caso contrário, a operação iniciará o processo de provisionamento de agendamento em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="28d5c-107">When clients use the [PUT method](team-put-schedule.md), if the schedule is provisioned, the operation updates the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="28d5c-108">Durante o provisionamento de agendamento, os clientes podem usar o método GET para obter o agendamento e observar a `provisionStatus` propriedade para o estado atual do provisionamento.</span><span class="sxs-lookup"><span data-stu-id="28d5c-108">During schedule provisioning, clients can use the GET method to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="28d5c-109">Se o provisionamento falhar, os clientes poderão obter informações adicionais da `provisionStatusCode` propriedade.</span><span class="sxs-lookup"><span data-stu-id="28d5c-109">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="28d5c-110">Os clientes também podem inspecionar a configuração do cronograma.</span><span class="sxs-lookup"><span data-stu-id="28d5c-110">Clients can also inspect the configuration of the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="28d5c-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="28d5c-111">Permissions</span></span>

<span data-ttu-id="28d5c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28d5c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28d5c-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28d5c-114">Permission type</span></span>      | <span data-ttu-id="28d5c-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28d5c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28d5c-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28d5c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="28d5c-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28d5c-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="28d5c-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28d5c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28d5c-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28d5c-119">Not supported.</span></span>    |
|<span data-ttu-id="28d5c-120">Application</span><span class="sxs-lookup"><span data-stu-id="28d5c-120">Application</span></span> | <span data-ttu-id="28d5c-121">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="28d5c-121">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="28d5c-122">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="28d5c-122">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="28d5c-123">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="28d5c-123">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="28d5c-124">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="28d5c-124">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="28d5c-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28d5c-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28d5c-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="28d5c-126">Optional query parameters</span></span>

<span data-ttu-id="28d5c-127">Este método não oferece suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="28d5c-127">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28d5c-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28d5c-128">Request headers</span></span>

| <span data-ttu-id="28d5c-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28d5c-129">Header</span></span>       | <span data-ttu-id="28d5c-130">Valor</span><span class="sxs-lookup"><span data-stu-id="28d5c-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="28d5c-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="28d5c-131">Authorization</span></span>  | <span data-ttu-id="28d5c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28d5c-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="28d5c-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28d5c-134">Content-Type</span></span>  | <span data-ttu-id="28d5c-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28d5c-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="28d5c-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28d5c-137">Request body</span></span>
<span data-ttu-id="28d5c-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28d5c-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28d5c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="28d5c-139">Response</span></span>

<span data-ttu-id="28d5c-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Schedule](../resources/schedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28d5c-140">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28d5c-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28d5c-141">Example</span></span>

#### <a name="request"></a><span data-ttu-id="28d5c-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28d5c-142">Request</span></span>

<span data-ttu-id="28d5c-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="28d5c-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28d5c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="28d5c-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule
```
# <a name="c"></a>[<span data-ttu-id="28d5c-145">C#</span><span class="sxs-lookup"><span data-stu-id="28d5c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28d5c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28d5c-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28d5c-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28d5c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="28d5c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="28d5c-148">Response</span></span>

<span data-ttu-id="28d5c-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="28d5c-149">The following is an example of the response.</span></span> 

><span data-ttu-id="28d5c-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28d5c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

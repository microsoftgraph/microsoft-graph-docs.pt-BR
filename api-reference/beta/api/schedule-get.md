---
title: Obter cronograma
description: Recupere as propriedades e os relacionamentos de um objeto **Schedule** .
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 550add9c5b74ce906a342051fafeb8a43b1a1415
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331371"
---
# <a name="get-schedule"></a><span data-ttu-id="788fa-103">Obter cronograma</span><span class="sxs-lookup"><span data-stu-id="788fa-103">Get schedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="788fa-104">Recupere as propriedades e os relacionamentos de um objeto [Schedule](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="788fa-104">Retrieve the properties and relationships of a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="788fa-105">O processo de criação de agendamento está em conformidade com a [diretriz de uma API para operações de longa duração com base em recursos (relo)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span><span class="sxs-lookup"><span data-stu-id="788fa-105">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="788fa-106">Quando os clientes usam o [método Put](team-put-schedule.md), se a agenda for provisionada, a operação atualizará a agenda; caso contrário, a operação iniciará o processo de provisionamento de agendamento em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="788fa-106">When clients use the [PUT method](team-put-schedule.md), if the schedule is provisioned, the operation updates the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="788fa-107">Durante o provisionamento de agendamento, os clientes podem usar o método GET para obter o agendamento e observar a `provisionStatus` propriedade para o estado atual do provisionamento.</span><span class="sxs-lookup"><span data-stu-id="788fa-107">During schedule provisioning, clients can use the GET method to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="788fa-108">Se o provisionamento falhar, os clientes poderão obter informações adicionais da `provisionStatusCode` propriedade.</span><span class="sxs-lookup"><span data-stu-id="788fa-108">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="788fa-109">Os clientes também podem inspecionar a configuração do cronograma.</span><span class="sxs-lookup"><span data-stu-id="788fa-109">Clients can also inspect the configuration of the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="788fa-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="788fa-110">Permissions</span></span>

<span data-ttu-id="788fa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="788fa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="788fa-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="788fa-113">Permission type</span></span>      | <span data-ttu-id="788fa-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="788fa-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="788fa-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="788fa-115">Delegated (work or school account)</span></span> | <span data-ttu-id="788fa-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="788fa-116">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="788fa-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="788fa-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="788fa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="788fa-118">Not supported.</span></span>    |
|<span data-ttu-id="788fa-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="788fa-119">Application</span></span> | <span data-ttu-id="788fa-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="788fa-120">Not supported.</span></span> |

> <span data-ttu-id="788fa-121">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="788fa-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="788fa-122">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="788fa-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="788fa-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="788fa-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="788fa-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="788fa-124">Request headers</span></span>

| <span data-ttu-id="788fa-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="788fa-125">Header</span></span>       | <span data-ttu-id="788fa-126">Valor</span><span class="sxs-lookup"><span data-stu-id="788fa-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="788fa-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="788fa-127">Authorization</span></span>  | <span data-ttu-id="788fa-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="788fa-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="788fa-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="788fa-130">Content-Type</span></span>  | <span data-ttu-id="788fa-131">application/json</span><span class="sxs-lookup"><span data-stu-id="788fa-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="788fa-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="788fa-132">Request body</span></span>
<span data-ttu-id="788fa-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="788fa-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="788fa-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="788fa-134">Response</span></span>

<span data-ttu-id="788fa-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Schedule](../resources/schedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="788fa-135">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="788fa-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="788fa-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="788fa-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="788fa-137">Request</span></span>

<span data-ttu-id="788fa-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="788fa-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule
```

#### <a name="response"></a><span data-ttu-id="788fa-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="788fa-139">Response</span></span>

<span data-ttu-id="788fa-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="788fa-140">The following is an example of the response.</span></span> 

><span data-ttu-id="788fa-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="788fa-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "provisionStatusCode": null
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
  "suppressions": []
}
-->

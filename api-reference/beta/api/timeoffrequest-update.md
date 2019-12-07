---
title: Atualizar timeoffrequest
description: Atualize as propriedades do objeto timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4e961a197620f27de11397952c2d868dcec848c3
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895524"
---
# <a name="update-timeoffrequest"></a><span data-ttu-id="a0299-103">Atualizar timeoffrequest</span><span class="sxs-lookup"><span data-stu-id="a0299-103">Update timeoffrequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0299-104">Atualize as propriedades do objeto [timeoffrequest](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="a0299-104">Update the properties of [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0299-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0299-105">Permissions</span></span>

<span data-ttu-id="a0299-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0299-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0299-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0299-108">Permission type</span></span>                        | <span data-ttu-id="a0299-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0299-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a0299-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0299-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0299-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0299-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="a0299-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0299-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0299-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0299-113">Not supported.</span></span> |
| <span data-ttu-id="a0299-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0299-114">Application</span></span>                            | <span data-ttu-id="a0299-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0299-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0299-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0299-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/timeOffRequests
```

## <a name="request-headers"></a><span data-ttu-id="a0299-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0299-117">Request headers</span></span>

| <span data-ttu-id="a0299-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a0299-118">Name</span></span>       | <span data-ttu-id="a0299-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0299-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a0299-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0299-120">Authorization</span></span> | <span data-ttu-id="a0299-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="a0299-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0299-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0299-122">Request body</span></span>

<span data-ttu-id="a0299-123">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="a0299-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a0299-124">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="a0299-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a0299-125">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a0299-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a0299-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0299-126">Property</span></span>     | <span data-ttu-id="a0299-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0299-127">Type</span></span>        | <span data-ttu-id="a0299-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0299-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a0299-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a0299-129">endDateTime</span></span>|<span data-ttu-id="a0299-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0299-130">DateTimeOffset</span></span>|<span data-ttu-id="a0299-131">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a0299-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a0299-132">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' ' 2014-01-01T00:00:00Z '</span><span class="sxs-lookup"><span data-stu-id="a0299-132">For example, midnight UTC on Jan 1, 2014 would look like this: \`'2014-01-01T00:00:00Z'</span></span>|
|<span data-ttu-id="a0299-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a0299-133">startDateTime</span></span>|<span data-ttu-id="a0299-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0299-134">DateTimeOffset</span></span>|<span data-ttu-id="a0299-135">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a0299-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a0299-136">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' ' 2014-01-01T00:00:00Z '</span><span class="sxs-lookup"><span data-stu-id="a0299-136">For example, midnight UTC on Jan 1, 2014 would look like this: \`'2014-01-01T00:00:00Z'</span></span>|
|<span data-ttu-id="a0299-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="a0299-137">timeOffReasonId</span></span>|<span data-ttu-id="a0299-138">String</span><span class="sxs-lookup"><span data-stu-id="a0299-138">String</span></span>|<span data-ttu-id="a0299-139">Razão para o tempo limite solicitado.</span><span class="sxs-lookup"><span data-stu-id="a0299-139">Reason for the requested time off.</span></span>|

## <a name="response"></a><span data-ttu-id="a0299-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0299-140">Response</span></span>

<span data-ttu-id="a0299-141">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [timeOffRequest](../resources/timeoffrequest.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0299-141">If successful, this method returns a `200 OK` response code and an updated [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0299-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a0299-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a0299-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0299-143">Request</span></span>

<span data-ttu-id="a0299-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0299-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_timeoffrequest"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests
Content-type: application/json

{
  "startDateTime": "datetime-value",
  "endDateTime": "datetime-value",
  "timeOffReasonId": "timeOffReasonId-value"
}
```

### <a name="response"></a><span data-ttu-id="a0299-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0299-145">Response</span></span>

<span data-ttu-id="a0299-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a0299-146">The following is an example of the response.</span></span>

> <span data-ttu-id="a0299-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0299-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "startDateTime": "datetime-value",
  "endDateTime": "datetime-value",
  "timeOffReasonId": "timeOffReasonId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update timeoffrequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
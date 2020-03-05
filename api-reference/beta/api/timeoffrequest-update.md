---
title: Atualizar timeoffrequest
description: Atualize as propriedades do objeto timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8d5a230f11bfd9d4727821d54f723a2e30de40be
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452243"
---
# <a name="update-timeoffrequest"></a><span data-ttu-id="5b329-103">Atualizar timeoffrequest</span><span class="sxs-lookup"><span data-stu-id="5b329-103">Update timeoffrequest</span></span>

<span data-ttu-id="5b329-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5b329-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b329-105">Atualiza as propriedades de um objeto [timeoffrequest](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="5b329-105">Update the properties of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b329-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b329-106">Permissions</span></span>

<span data-ttu-id="5b329-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b329-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b329-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b329-109">Permission type</span></span>                        | <span data-ttu-id="5b329-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b329-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5b329-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b329-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b329-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b329-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="5b329-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b329-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b329-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b329-114">Not supported.</span></span> |
|<span data-ttu-id="5b329-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b329-115">Application</span></span> | <span data-ttu-id="5b329-116">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="5b329-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="5b329-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="5b329-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="5b329-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b329-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/timeOffRequests
```

## <a name="request-headers"></a><span data-ttu-id="5b329-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b329-119">Request headers</span></span>

| <span data-ttu-id="5b329-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5b329-120">Name</span></span>       | <span data-ttu-id="5b329-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b329-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5b329-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b329-122">Authorization</span></span> | <span data-ttu-id="5b329-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b329-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b329-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="5b329-125">Content-type</span></span> | <span data-ttu-id="5b329-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b329-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b329-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b329-128">Request body</span></span>

<span data-ttu-id="5b329-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="5b329-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5b329-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="5b329-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5b329-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5b329-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5b329-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b329-132">Property</span></span>     | <span data-ttu-id="5b329-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b329-133">Type</span></span>        | <span data-ttu-id="5b329-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b329-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5b329-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5b329-135">endDateTime</span></span>|<span data-ttu-id="5b329-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b329-136">DateTimeOffset</span></span>|<span data-ttu-id="5b329-137">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5b329-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5b329-138">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' ' 2014-01-01T00:00:00Z '</span><span class="sxs-lookup"><span data-stu-id="5b329-138">For example, midnight UTC on Jan 1, 2014 would look like this: \`'2014-01-01T00:00:00Z'</span></span>|
|<span data-ttu-id="5b329-139">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5b329-139">startDateTime</span></span>|<span data-ttu-id="5b329-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b329-140">DateTimeOffset</span></span>|<span data-ttu-id="5b329-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5b329-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5b329-142">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' ' 2014-01-01T00:00:00Z '</span><span class="sxs-lookup"><span data-stu-id="5b329-142">For example, midnight UTC on Jan 1, 2014 would look like this: \`'2014-01-01T00:00:00Z'</span></span>|
|<span data-ttu-id="5b329-143">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="5b329-143">timeOffReasonId</span></span>|<span data-ttu-id="5b329-144">String</span><span class="sxs-lookup"><span data-stu-id="5b329-144">String</span></span>|<span data-ttu-id="5b329-145">Razão para o tempo limite solicitado.</span><span class="sxs-lookup"><span data-stu-id="5b329-145">Reason for the requested time off.</span></span>|

## <a name="response"></a><span data-ttu-id="5b329-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b329-146">Response</span></span>

<span data-ttu-id="5b329-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [timeOffRequest](../resources/timeoffrequest.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b329-147">If successful, this method returns a `200 OK` response code and an updated [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b329-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5b329-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b329-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b329-149">Request</span></span>

<span data-ttu-id="5b329-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b329-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5b329-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b329-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5b329-152">C#</span><span class="sxs-lookup"><span data-stu-id="5b329-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b329-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b329-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b329-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b329-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5b329-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b329-155">Response</span></span>

<span data-ttu-id="5b329-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5b329-156">The following is an example of the response.</span></span>

> <span data-ttu-id="5b329-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b329-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

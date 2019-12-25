---
title: Atualizar timeoffrequest
description: Atualize as propriedades do objeto timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2197e0e4e2f9c78337a6d5ae06d6c1e106f77afa
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863523"
---
# <a name="update-timeoffrequest"></a><span data-ttu-id="d333f-103">Atualizar timeoffrequest</span><span class="sxs-lookup"><span data-stu-id="d333f-103">Update timeoffrequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d333f-104">Atualiza as propriedades de um objeto [timeoffrequest](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="d333f-104">Update the properties of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d333f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d333f-105">Permissions</span></span>

<span data-ttu-id="d333f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d333f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d333f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d333f-108">Permission type</span></span>                        | <span data-ttu-id="d333f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d333f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d333f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d333f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d333f-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d333f-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d333f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d333f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d333f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d333f-113">Not supported.</span></span> |
|<span data-ttu-id="d333f-114">Application</span><span class="sxs-lookup"><span data-stu-id="d333f-114">Application</span></span> | <span data-ttu-id="d333f-115">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="d333f-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="d333f-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="d333f-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="d333f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d333f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/timeOffRequests
```

## <a name="request-headers"></a><span data-ttu-id="d333f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d333f-118">Request headers</span></span>

| <span data-ttu-id="d333f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d333f-119">Name</span></span>       | <span data-ttu-id="d333f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d333f-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d333f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d333f-121">Authorization</span></span> | <span data-ttu-id="d333f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d333f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d333f-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="d333f-124">Content-type</span></span> | <span data-ttu-id="d333f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d333f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d333f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d333f-127">Request body</span></span>

<span data-ttu-id="d333f-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="d333f-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d333f-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d333f-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d333f-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d333f-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d333f-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d333f-131">Property</span></span>     | <span data-ttu-id="d333f-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d333f-132">Type</span></span>        | <span data-ttu-id="d333f-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d333f-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d333f-134">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d333f-134">endDateTime</span></span>|<span data-ttu-id="d333f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d333f-135">DateTimeOffset</span></span>|<span data-ttu-id="d333f-136">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d333f-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d333f-137">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' ' 2014-01-01T00:00:00Z '</span><span class="sxs-lookup"><span data-stu-id="d333f-137">For example, midnight UTC on Jan 1, 2014 would look like this: \`'2014-01-01T00:00:00Z'</span></span>|
|<span data-ttu-id="d333f-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d333f-138">startDateTime</span></span>|<span data-ttu-id="d333f-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d333f-139">DateTimeOffset</span></span>|<span data-ttu-id="d333f-140">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d333f-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d333f-141">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' ' 2014-01-01T00:00:00Z '</span><span class="sxs-lookup"><span data-stu-id="d333f-141">For example, midnight UTC on Jan 1, 2014 would look like this: \`'2014-01-01T00:00:00Z'</span></span>|
|<span data-ttu-id="d333f-142">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="d333f-142">timeOffReasonId</span></span>|<span data-ttu-id="d333f-143">String</span><span class="sxs-lookup"><span data-stu-id="d333f-143">String</span></span>|<span data-ttu-id="d333f-144">Razão para o tempo limite solicitado.</span><span class="sxs-lookup"><span data-stu-id="d333f-144">Reason for the requested time off.</span></span>|

## <a name="response"></a><span data-ttu-id="d333f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d333f-145">Response</span></span>

<span data-ttu-id="d333f-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [timeOffRequest](../resources/timeoffrequest.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d333f-146">If successful, this method returns a `200 OK` response code and an updated [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d333f-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d333f-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d333f-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d333f-148">Request</span></span>

<span data-ttu-id="d333f-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d333f-149">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d333f-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="d333f-150">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d333f-151">C#</span><span class="sxs-lookup"><span data-stu-id="d333f-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d333f-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d333f-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d333f-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d333f-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d333f-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d333f-154">Response</span></span>

<span data-ttu-id="d333f-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d333f-155">The following is an example of the response.</span></span>

> <span data-ttu-id="d333f-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d333f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

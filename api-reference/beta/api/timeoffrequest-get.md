---
title: Obter timeOffRequest
description: Recupere as propriedades e os relacionamentos do objeto timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 267710b78fed5abfb83e7c9492c7bdff603b91d3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058596"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="2e350-103">Obter timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="2e350-103">Get timeOffRequest</span></span>

<span data-ttu-id="2e350-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e350-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e350-105">Recupere as propriedades e os relacionamentos de um objeto [timeoffrequest](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="2e350-105">Retrieve the properties and relationships of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e350-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e350-106">Permissions</span></span>

<span data-ttu-id="2e350-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e350-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e350-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e350-109">Permission type</span></span>                        | <span data-ttu-id="2e350-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e350-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2e350-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e350-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e350-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e350-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="2e350-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e350-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e350-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e350-114">Not supported.</span></span> |
|<span data-ttu-id="2e350-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e350-115">Application</span></span> | <span data-ttu-id="2e350-116">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="2e350-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="2e350-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="2e350-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="2e350-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e350-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e350-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2e350-119">Optional query parameters</span></span>

<span data-ttu-id="2e350-120">Este método não oferece suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2e350-120">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e350-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e350-121">Request headers</span></span>

| <span data-ttu-id="2e350-122">Nome</span><span class="sxs-lookup"><span data-stu-id="2e350-122">Name</span></span>      |<span data-ttu-id="2e350-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e350-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2e350-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e350-124">Authorization</span></span> | <span data-ttu-id="2e350-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e350-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e350-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e350-127">Request body</span></span>

<span data-ttu-id="2e350-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e350-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e350-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e350-129">Response</span></span>

<span data-ttu-id="2e350-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [timeOffRequest](../resources/timeoffrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e350-130">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e350-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2e350-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e350-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e350-132">Request</span></span>

<span data-ttu-id="2e350-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e350-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e350-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e350-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="2e350-135">C#</span><span class="sxs-lookup"><span data-stu-id="2e350-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e350-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e350-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e350-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e350-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2e350-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e350-138">Response</span></span>

<span data-ttu-id="2e350-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2e350-139">The following is an example of the response.</span></span>

> <span data-ttu-id="2e350-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e350-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Get timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



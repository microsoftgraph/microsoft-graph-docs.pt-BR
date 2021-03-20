---
title: Obter timeOffRequest
description: Recupere as propriedades e as relações do objeto timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 187dfaeeb6888c9717f6270166cbee61c6816082
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953897"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="38bde-103">Obter timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="38bde-103">Get timeOffRequest</span></span>

<span data-ttu-id="38bde-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38bde-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38bde-105">Recupere as propriedades e as relações de um [objeto timeoffrequest.](../resources/timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="38bde-105">Retrieve the properties and relationships of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="38bde-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="38bde-106">Permissions</span></span>

<span data-ttu-id="38bde-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38bde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38bde-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38bde-109">Permission type</span></span>                        | <span data-ttu-id="38bde-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38bde-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="38bde-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38bde-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="38bde-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38bde-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="38bde-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38bde-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38bde-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38bde-114">Not supported.</span></span> |
|<span data-ttu-id="38bde-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38bde-115">Application</span></span> | <span data-ttu-id="38bde-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="38bde-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="38bde-117">\***Importante:** As permissões de aplicativo estão atualmente apenas em visualização privada e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="38bde-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="38bde-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38bde-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38bde-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="38bde-119">Optional query parameters</span></span>

<span data-ttu-id="38bde-120">Este método não dá suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="38bde-120">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38bde-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38bde-121">Request headers</span></span>

| <span data-ttu-id="38bde-122">Nome</span><span class="sxs-lookup"><span data-stu-id="38bde-122">Name</span></span>      |<span data-ttu-id="38bde-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="38bde-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="38bde-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="38bde-124">Authorization</span></span> | <span data-ttu-id="38bde-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38bde-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38bde-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38bde-127">Request body</span></span>

<span data-ttu-id="38bde-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38bde-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38bde-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="38bde-129">Response</span></span>

<span data-ttu-id="38bde-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [timeOffRequest](../resources/timeoffrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38bde-130">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="38bde-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="38bde-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="38bde-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38bde-132">Request</span></span>

<span data-ttu-id="38bde-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38bde-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="38bde-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="38bde-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="38bde-135">C#</span><span class="sxs-lookup"><span data-stu-id="38bde-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38bde-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38bde-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38bde-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38bde-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38bde-138">Java</span><span class="sxs-lookup"><span data-stu-id="38bde-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-timeoffrequest-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="38bde-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="38bde-139">Response</span></span>

<span data-ttu-id="38bde-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="38bde-140">The following is an example of the response.</span></span>

> <span data-ttu-id="38bde-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38bde-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



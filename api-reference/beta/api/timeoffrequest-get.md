---
title: Obter timeOffRequest
description: Recupere as propriedades e as relações do objeto timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c961704a21112dbd738102ea0ab14c81bbd3a28f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048936"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="c986b-103">Obter timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="c986b-103">Get timeOffRequest</span></span>

<span data-ttu-id="c986b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c986b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c986b-105">Recupere as propriedades e as relações de um [objeto timeoffrequest.](../resources/timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="c986b-105">Retrieve the properties and relationships of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c986b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c986b-106">Permissions</span></span>

<span data-ttu-id="c986b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c986b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c986b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c986b-109">Permission type</span></span>                        | <span data-ttu-id="c986b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c986b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c986b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c986b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c986b-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c986b-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c986b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c986b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c986b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c986b-114">Not supported.</span></span> |
|<span data-ttu-id="c986b-115">Application</span><span class="sxs-lookup"><span data-stu-id="c986b-115">Application</span></span> | <span data-ttu-id="c986b-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="c986b-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="c986b-117">\***Importante:** As permissões de aplicativo estão atualmente apenas em visualização privada e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="c986b-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="c986b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c986b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c986b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c986b-119">Optional query parameters</span></span>

<span data-ttu-id="c986b-120">Este método não dá suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c986b-120">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c986b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c986b-121">Request headers</span></span>

| <span data-ttu-id="c986b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c986b-122">Name</span></span>      |<span data-ttu-id="c986b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c986b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c986b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c986b-124">Authorization</span></span> | <span data-ttu-id="c986b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c986b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c986b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c986b-127">Request body</span></span>

<span data-ttu-id="c986b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c986b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c986b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c986b-129">Response</span></span>

<span data-ttu-id="c986b-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [timeOffRequest](../resources/timeoffrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c986b-130">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c986b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c986b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c986b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c986b-132">Request</span></span>

<span data-ttu-id="c986b-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c986b-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c986b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c986b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="c986b-135">C#</span><span class="sxs-lookup"><span data-stu-id="c986b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c986b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c986b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c986b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c986b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c986b-138">Java</span><span class="sxs-lookup"><span data-stu-id="c986b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-timeoffrequest-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c986b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c986b-139">Response</span></span>

<span data-ttu-id="c986b-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c986b-140">The following is an example of the response.</span></span>

> <span data-ttu-id="c986b-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c986b-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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



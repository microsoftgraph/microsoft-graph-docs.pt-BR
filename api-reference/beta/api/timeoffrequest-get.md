---
title: Obter timeOffRequest
description: Recupere as propriedades e os relacionamentos do objeto timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1036ef42706c95cd5aeada2db32f7bd6ffffd110
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452250"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="1081a-103">Obter timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="1081a-103">Get timeOffRequest</span></span>

<span data-ttu-id="1081a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1081a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1081a-105">Recupere as propriedades e os relacionamentos de um objeto [timeoffrequest](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="1081a-105">Retrieve the properties and relationships of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1081a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1081a-106">Permissions</span></span>

<span data-ttu-id="1081a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1081a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1081a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1081a-109">Permission type</span></span>                        | <span data-ttu-id="1081a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1081a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1081a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1081a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1081a-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1081a-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1081a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1081a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1081a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1081a-114">Not supported.</span></span> |
|<span data-ttu-id="1081a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1081a-115">Application</span></span> | <span data-ttu-id="1081a-116">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="1081a-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="1081a-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="1081a-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="1081a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1081a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/timeOffRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1081a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1081a-119">Optional query parameters</span></span>

<span data-ttu-id="1081a-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1081a-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1081a-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1081a-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1081a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1081a-122">Request headers</span></span>

| <span data-ttu-id="1081a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1081a-123">Name</span></span>      |<span data-ttu-id="1081a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1081a-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1081a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1081a-125">Authorization</span></span> | <span data-ttu-id="1081a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1081a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1081a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1081a-128">Request body</span></span>

<span data-ttu-id="1081a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1081a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1081a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1081a-130">Response</span></span>

<span data-ttu-id="1081a-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [timeOffRequest](../resources/timeoffrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1081a-131">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1081a-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1081a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1081a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1081a-133">Request</span></span>

<span data-ttu-id="1081a-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1081a-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1081a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1081a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests
```
# <a name="c"></a>[<span data-ttu-id="1081a-136">C#</span><span class="sxs-lookup"><span data-stu-id="1081a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1081a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1081a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1081a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1081a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1081a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1081a-139">Response</span></span>

<span data-ttu-id="1081a-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1081a-140">The following is an example of the response.</span></span>

> <span data-ttu-id="1081a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1081a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

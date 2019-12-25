---
title: Obter timeOffRequest
description: Recupere as propriedades e os relacionamentos do objeto timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2f8cfce33bd0945cd06c573d9182ed49b943640a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863552"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="b46f9-103">Obter timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="b46f9-103">Get timeOffRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b46f9-104">Recupere as propriedades e os relacionamentos de um objeto [timeoffrequest](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="b46f9-104">Retrieve the properties and relationships of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b46f9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b46f9-105">Permissions</span></span>

<span data-ttu-id="b46f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b46f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b46f9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b46f9-108">Permission type</span></span>                        | <span data-ttu-id="b46f9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b46f9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b46f9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b46f9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b46f9-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b46f9-111">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="b46f9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b46f9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b46f9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b46f9-113">Not supported.</span></span> |
|<span data-ttu-id="b46f9-114">Application</span><span class="sxs-lookup"><span data-stu-id="b46f9-114">Application</span></span> | <span data-ttu-id="b46f9-115">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="b46f9-115">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="b46f9-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="b46f9-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="b46f9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b46f9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/timeOffRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b46f9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b46f9-118">Optional query parameters</span></span>

<span data-ttu-id="b46f9-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b46f9-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b46f9-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b46f9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b46f9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b46f9-121">Request headers</span></span>

| <span data-ttu-id="b46f9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b46f9-122">Name</span></span>      |<span data-ttu-id="b46f9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b46f9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b46f9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b46f9-124">Authorization</span></span> | <span data-ttu-id="b46f9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b46f9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b46f9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b46f9-127">Request body</span></span>

<span data-ttu-id="b46f9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b46f9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b46f9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b46f9-129">Response</span></span>

<span data-ttu-id="b46f9-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [timeOffRequest](../resources/timeoffrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b46f9-130">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b46f9-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b46f9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b46f9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b46f9-132">Request</span></span>

<span data-ttu-id="b46f9-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b46f9-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b46f9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b46f9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b46f9-135">C#</span><span class="sxs-lookup"><span data-stu-id="b46f9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b46f9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b46f9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b46f9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b46f9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b46f9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b46f9-138">Response</span></span>

<span data-ttu-id="b46f9-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b46f9-139">The following is an example of the response.</span></span>

> <span data-ttu-id="b46f9-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b46f9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

---
title: Obter timeOffRequest
description: Recupere as propriedades e os relacionamentos do objeto timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 29c2ac88bf1253d3a00a395d990f1974bda50815
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895520"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="23f82-103">Obter timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="23f82-103">Get timeOffRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23f82-104">Recupere as propriedades e os relacionamentos do objeto [timeoffrequest](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="23f82-104">Retrieve the properties and relationships of [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="23f82-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="23f82-105">Permissions</span></span>

<span data-ttu-id="23f82-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23f82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23f82-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23f82-108">Permission type</span></span>                        | <span data-ttu-id="23f82-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23f82-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="23f82-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23f82-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="23f82-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23f82-111">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="23f82-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23f82-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23f82-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23f82-113">Not supported.</span></span> |
| <span data-ttu-id="23f82-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23f82-114">Application</span></span>                            | <span data-ttu-id="23f82-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23f82-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="23f82-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23f82-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/timeOffRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23f82-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="23f82-117">Optional query parameters</span></span>

<span data-ttu-id="23f82-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="23f82-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="23f82-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="23f82-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="23f82-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23f82-120">Request headers</span></span>

| <span data-ttu-id="23f82-121">Nome</span><span class="sxs-lookup"><span data-stu-id="23f82-121">Name</span></span>      |<span data-ttu-id="23f82-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="23f82-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="23f82-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="23f82-123">Authorization</span></span> | <span data-ttu-id="23f82-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="23f82-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="23f82-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23f82-125">Request body</span></span>

<span data-ttu-id="23f82-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23f82-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23f82-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="23f82-127">Response</span></span>

<span data-ttu-id="23f82-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [timeOffRequest](../resources/timeoffrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23f82-128">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="23f82-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="23f82-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="23f82-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23f82-130">Request</span></span>

<span data-ttu-id="23f82-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="23f82-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests
```

### <a name="response"></a><span data-ttu-id="23f82-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="23f82-132">Response</span></span>

<span data-ttu-id="23f82-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="23f82-133">The following is an example of the response.</span></span>

> <span data-ttu-id="23f82-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23f82-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
---
title: Obter swapShiftsChangeRequest
description: Recupere as propriedades e os relacionamentos de um objeto swapShiftsChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d0968813f16ff4280bcd2319495ceeb98572df6f
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895538"
---
# <a name="get-swapshiftschangerequest"></a><span data-ttu-id="e24d9-103">Obter swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="e24d9-103">Get swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e24d9-104">Recupere as propriedades e os relacionamentos de um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="e24d9-104">Retrieve the properties and relationships of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e24d9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e24d9-105">Permissions</span></span>

<span data-ttu-id="e24d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e24d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e24d9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e24d9-108">Permission type</span></span>                        | <span data-ttu-id="e24d9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e24d9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e24d9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e24d9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e24d9-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e24d9-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="e24d9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e24d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e24d9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e24d9-113">Not supported.</span></span> |
| <span data-ttu-id="e24d9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e24d9-114">Application</span></span>                            | <span data-ttu-id="e24d9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e24d9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e24d9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e24d9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e24d9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e24d9-117">Optional query parameters</span></span>

<span data-ttu-id="e24d9-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e24d9-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e24d9-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e24d9-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e24d9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e24d9-120">Request headers</span></span>

| <span data-ttu-id="e24d9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e24d9-121">Name</span></span>      |<span data-ttu-id="e24d9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e24d9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e24d9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e24d9-123">Authorization</span></span> | <span data-ttu-id="e24d9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e24d9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e24d9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e24d9-126">Request body</span></span>

<span data-ttu-id="e24d9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e24d9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e24d9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e24d9-128">Response</span></span>

<span data-ttu-id="e24d9-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e24d9-129">If successful, this method returns a `200 OK` response code and the requested [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e24d9-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e24d9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e24d9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e24d9-131">Request</span></span>

<span data-ttu-id="e24d9-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e24d9-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_swapshiftschangerequest"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests
```

### <a name="response"></a><span data-ttu-id="e24d9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e24d9-133">Response</span></span>

<span data-ttu-id="e24d9-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e24d9-134">The following is an example of the response.</span></span>

> <span data-ttu-id="e24d9-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e24d9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "recipientShiftId": "recipientShiftId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get swapShiftsChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

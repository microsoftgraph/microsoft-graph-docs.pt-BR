---
title: Obter offerShiftRequest
description: Recupere as propriedades e os relacionamentos de um objeto offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 20bfcafa501872e84d91549b3723029298119add
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44153540"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="2f18b-103">Obter offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="2f18b-103">Get offerShiftRequest</span></span>

<span data-ttu-id="2f18b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f18b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f18b-105">Recupere as propriedades e os relacionamentos de um objeto [offerShiftRequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="2f18b-105">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f18b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f18b-106">Permissions</span></span>

<span data-ttu-id="2f18b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f18b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f18b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f18b-109">Permission type</span></span>                        | <span data-ttu-id="2f18b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f18b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2f18b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f18b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f18b-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f18b-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="2f18b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f18b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f18b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f18b-114">Not supported.</span></span> |
| <span data-ttu-id="2f18b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f18b-115">Application</span></span>                            | <span data-ttu-id="2f18b-116">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="2f18b-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="2f18b-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="2f18b-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="2f18b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f18b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f18b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2f18b-119">Optional query parameters</span></span>

<span data-ttu-id="2f18b-120">Este método não oferece suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2f18b-120">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f18b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f18b-121">Request headers</span></span>

| <span data-ttu-id="2f18b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="2f18b-122">Name</span></span>      |<span data-ttu-id="2f18b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f18b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2f18b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f18b-124">Authorization</span></span> | <span data-ttu-id="2f18b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f18b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f18b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f18b-127">Request body</span></span>

<span data-ttu-id="2f18b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f18b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f18b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f18b-129">Response</span></span>

<span data-ttu-id="2f18b-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [offerShiftRequest](../resources/offershiftrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f18b-130">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f18b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2f18b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2f18b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f18b-132">Request</span></span>

<span data-ttu-id="2f18b-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f18b-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2f18b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f18b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```
# <a name="c"></a>[<span data-ttu-id="2f18b-135">C#</span><span class="sxs-lookup"><span data-stu-id="2f18b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f18b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f18b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f18b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f18b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2f18b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f18b-138">Response</span></span>

<span data-ttu-id="2f18b-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f18b-139">The following is an example of the response.</span></span>

> <span data-ttu-id="2f18b-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f18b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "recipientActionMessage": "recipientActionMessage-value",
  "recipientActionDateTime": "datetime-value",
  "senderShiftId": "senderShiftId-value",
  "recipientUserId": "recipientUserId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get offerShiftRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

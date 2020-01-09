---
title: Obter offerShiftRequest
description: Recupere as propriedades e os relacionamentos de um objeto offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d029254a3ccc3f125064aaa3708055ac70d16d13
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994919"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="32876-103">Obter offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="32876-103">Get offerShiftRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32876-104">Recupere as propriedades e os relacionamentos de um objeto [offerShiftRequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="32876-104">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="32876-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="32876-105">Permissions</span></span>

<span data-ttu-id="32876-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32876-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32876-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32876-108">Permission type</span></span>                        | <span data-ttu-id="32876-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32876-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="32876-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32876-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="32876-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32876-111">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="32876-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32876-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32876-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32876-113">Not supported.</span></span> |
| <span data-ttu-id="32876-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32876-114">Application</span></span>                            | <span data-ttu-id="32876-115">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="32876-115">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="32876-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="32876-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="32876-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32876-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="32876-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="32876-118">Optional query parameters</span></span>

<span data-ttu-id="32876-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="32876-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="32876-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="32876-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="32876-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32876-121">Request headers</span></span>

| <span data-ttu-id="32876-122">Nome</span><span class="sxs-lookup"><span data-stu-id="32876-122">Name</span></span>      |<span data-ttu-id="32876-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="32876-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="32876-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="32876-124">Authorization</span></span> | <span data-ttu-id="32876-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32876-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32876-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32876-127">Request body</span></span>

<span data-ttu-id="32876-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32876-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32876-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="32876-129">Response</span></span>

<span data-ttu-id="32876-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [offerShiftRequest](../resources/offershiftrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32876-130">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="32876-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="32876-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="32876-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32876-132">Request</span></span>

<span data-ttu-id="32876-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="32876-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="32876-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="32876-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/schedule/offerShiftRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="32876-135">C#</span><span class="sxs-lookup"><span data-stu-id="32876-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="32876-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32876-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="32876-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32876-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="32876-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="32876-138">Response</span></span>

<span data-ttu-id="32876-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="32876-139">The following is an example of the response.</span></span>

> <span data-ttu-id="32876-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32876-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

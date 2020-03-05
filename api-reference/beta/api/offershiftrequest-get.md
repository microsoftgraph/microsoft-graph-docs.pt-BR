---
title: Obter offerShiftRequest
description: Recupere as propriedades e os relacionamentos de um objeto offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c1ae04f4e2cd97cca0ad0f7c7719c4f1b6d4b5c5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456582"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="852f7-103">Obter offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="852f7-103">Get offerShiftRequest</span></span>

<span data-ttu-id="852f7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="852f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="852f7-105">Recupere as propriedades e os relacionamentos de um objeto [offerShiftRequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="852f7-105">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="852f7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="852f7-106">Permissions</span></span>

<span data-ttu-id="852f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="852f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="852f7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="852f7-109">Permission type</span></span>                        | <span data-ttu-id="852f7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="852f7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="852f7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="852f7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="852f7-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="852f7-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="852f7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="852f7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="852f7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="852f7-114">Not supported.</span></span> |
| <span data-ttu-id="852f7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="852f7-115">Application</span></span>                            | <span data-ttu-id="852f7-116">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="852f7-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="852f7-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="852f7-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="852f7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="852f7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="852f7-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="852f7-119">Optional query parameters</span></span>

<span data-ttu-id="852f7-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="852f7-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="852f7-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="852f7-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="852f7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="852f7-122">Request headers</span></span>

| <span data-ttu-id="852f7-123">Nome</span><span class="sxs-lookup"><span data-stu-id="852f7-123">Name</span></span>      |<span data-ttu-id="852f7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="852f7-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="852f7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="852f7-125">Authorization</span></span> | <span data-ttu-id="852f7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="852f7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="852f7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="852f7-128">Request body</span></span>

<span data-ttu-id="852f7-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="852f7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="852f7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="852f7-130">Response</span></span>

<span data-ttu-id="852f7-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [offerShiftRequest](../resources/offershiftrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="852f7-131">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="852f7-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="852f7-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="852f7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="852f7-133">Request</span></span>

<span data-ttu-id="852f7-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="852f7-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="852f7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="852f7-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/schedule/offerShiftRequests
```
# <a name="c"></a>[<span data-ttu-id="852f7-136">C#</span><span class="sxs-lookup"><span data-stu-id="852f7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="852f7-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="852f7-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="852f7-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="852f7-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="852f7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="852f7-139">Response</span></span>

<span data-ttu-id="852f7-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="852f7-140">The following is an example of the response.</span></span>

> <span data-ttu-id="852f7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="852f7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

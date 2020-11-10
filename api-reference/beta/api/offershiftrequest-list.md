---
title: Listar offerShiftRequest
description: Recupere as propriedades e os relacionamentos de todos os objetos offerShiftRequest de uma equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 244c96b26cc55ac4cc727979517ab5ce75b0c509
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981283"
---
# <a name="list-offershiftrequest"></a><span data-ttu-id="1157b-103">Listar offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="1157b-103">List offerShiftRequest</span></span>

<span data-ttu-id="1157b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1157b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1157b-105">Recupere as propriedades e os relacionamentos de todos os objetos [offerShiftRequest](../resources/offershiftrequest.md) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="1157b-105">Retrieve the properties and relationships of all [offerShiftRequest](../resources/offershiftrequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="1157b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1157b-106">Permissions</span></span>

<span data-ttu-id="1157b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1157b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1157b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1157b-109">Permission type</span></span>                        | <span data-ttu-id="1157b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1157b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1157b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1157b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1157b-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1157b-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1157b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1157b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1157b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1157b-114">Not supported.</span></span> |
| <span data-ttu-id="1157b-115">Application</span><span class="sxs-lookup"><span data-stu-id="1157b-115">Application</span></span>                            | <span data-ttu-id="1157b-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1157b-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1157b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1157b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1157b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1157b-118">Optional query parameters</span></span>

<span data-ttu-id="1157b-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1157b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1157b-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1157b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1157b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1157b-121">Request headers</span></span>

| <span data-ttu-id="1157b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1157b-122">Name</span></span>      |<span data-ttu-id="1157b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1157b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1157b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1157b-124">Authorization</span></span> | <span data-ttu-id="1157b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1157b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1157b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1157b-127">Request body</span></span>

<span data-ttu-id="1157b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1157b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1157b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1157b-129">Response</span></span>

<span data-ttu-id="1157b-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [offerShiftRequest](../resources/offershiftrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1157b-130">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1157b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1157b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1157b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1157b-132">Request</span></span>

<span data-ttu-id="1157b-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1157b-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1157b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1157b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests
```
# <a name="c"></a>[<span data-ttu-id="1157b-135">C#</span><span class="sxs-lookup"><span data-stu-id="1157b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1157b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1157b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1157b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1157b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1157b-138">Java</span><span class="sxs-lookup"><span data-stu-id="1157b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1157b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1157b-139">Response</span></span>

<span data-ttu-id="1157b-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1157b-140">The following is an example of the response.</span></span>

> <span data-ttu-id="1157b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1157b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



---
title: Listar offerShiftRequest
description: Recupere as propriedades e as relações de todos os objetos offerShiftRequest em uma equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aff40c4a4801fd7f9cb6229f0073d9f7247f81e6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038275"
---
# <a name="list-offershiftrequest"></a><span data-ttu-id="6efe7-103">Listar offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="6efe7-103">List offerShiftRequest</span></span>

<span data-ttu-id="6efe7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6efe7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6efe7-105">Recupere as propriedades e as relações de todos os [objetos offerShiftRequest](../resources/offershiftrequest.md) em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="6efe7-105">Retrieve the properties and relationships of all [offerShiftRequest](../resources/offershiftrequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="6efe7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6efe7-106">Permissions</span></span>

<span data-ttu-id="6efe7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6efe7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6efe7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6efe7-109">Permission type</span></span>                        | <span data-ttu-id="6efe7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6efe7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6efe7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6efe7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6efe7-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6efe7-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="6efe7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6efe7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6efe7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6efe7-114">Not supported.</span></span> |
| <span data-ttu-id="6efe7-115">Application</span><span class="sxs-lookup"><span data-stu-id="6efe7-115">Application</span></span>                            | <span data-ttu-id="6efe7-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6efe7-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6efe7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6efe7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6efe7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6efe7-118">Optional query parameters</span></span>

<span data-ttu-id="6efe7-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6efe7-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6efe7-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6efe7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6efe7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6efe7-121">Request headers</span></span>

| <span data-ttu-id="6efe7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6efe7-122">Name</span></span>      |<span data-ttu-id="6efe7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6efe7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6efe7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6efe7-124">Authorization</span></span> | <span data-ttu-id="6efe7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6efe7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6efe7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6efe7-127">Request body</span></span>

<span data-ttu-id="6efe7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6efe7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6efe7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6efe7-129">Response</span></span>

<span data-ttu-id="6efe7-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [offerShiftRequest](../resources/offershiftrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6efe7-130">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6efe7-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6efe7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6efe7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6efe7-132">Request</span></span>

<span data-ttu-id="6efe7-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6efe7-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6efe7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6efe7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests
```
# <a name="c"></a>[<span data-ttu-id="6efe7-135">C#</span><span class="sxs-lookup"><span data-stu-id="6efe7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6efe7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6efe7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6efe7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6efe7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6efe7-138">Java</span><span class="sxs-lookup"><span data-stu-id="6efe7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6efe7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6efe7-139">Response</span></span>

<span data-ttu-id="6efe7-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6efe7-140">The following is an example of the response.</span></span>

> <span data-ttu-id="6efe7-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6efe7-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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



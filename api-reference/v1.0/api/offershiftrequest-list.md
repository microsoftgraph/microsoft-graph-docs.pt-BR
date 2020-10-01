---
title: Listar offerShiftRequest
description: Recupere as propriedades e os relacionamentos de todos os objetos offerShiftRequest de uma equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: eaf553618bf044d0ecda13e40b19bc6a777c28c6
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313629"
---
# <a name="list-offershiftrequest"></a><span data-ttu-id="7347a-103">Listar offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="7347a-103">List offerShiftRequest</span></span>

<span data-ttu-id="7347a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7347a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7347a-105">Recupere as propriedades e os relacionamentos de todos os objetos [offerShiftRequest](../resources/offershiftrequest.md) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="7347a-105">Retrieve the properties and relationships of all [offerShiftRequest](../resources/offershiftrequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="7347a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7347a-106">Permissions</span></span>

<span data-ttu-id="7347a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7347a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7347a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7347a-109">Permission type</span></span>                        | <span data-ttu-id="7347a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7347a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7347a-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7347a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7347a-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7347a-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="7347a-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7347a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7347a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7347a-114">Not supported.</span></span> |
| <span data-ttu-id="7347a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7347a-115">Application</span></span>                            | <span data-ttu-id="7347a-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7347a-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7347a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7347a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7347a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7347a-118">Optional query parameters</span></span>

<span data-ttu-id="7347a-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7347a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7347a-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7347a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7347a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7347a-121">Request headers</span></span>

| <span data-ttu-id="7347a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7347a-122">Name</span></span>      |<span data-ttu-id="7347a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7347a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7347a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7347a-124">Authorization</span></span> | <span data-ttu-id="7347a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7347a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7347a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7347a-127">Request body</span></span>

<span data-ttu-id="7347a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7347a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7347a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7347a-129">Response</span></span>

<span data-ttu-id="7347a-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e os objetos [offerShiftRequest](../resources/offershiftrequest.md) solicitados no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7347a-130">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7347a-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7347a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7347a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7347a-132">Request</span></span>

<span data-ttu-id="7347a-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7347a-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7347a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7347a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests
```
# <a name="c"></a>[<span data-ttu-id="7347a-135">C#</span><span class="sxs-lookup"><span data-stu-id="7347a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7347a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7347a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7347a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7347a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7347a-138">Java</span><span class="sxs-lookup"><span data-stu-id="7347a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="7347a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7347a-139">Response</span></span>

<span data-ttu-id="7347a-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7347a-140">The following is an example of the response.</span></span>

> <span data-ttu-id="7347a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7347a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


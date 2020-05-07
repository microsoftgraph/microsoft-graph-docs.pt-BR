---
title: Listar offerShiftRequest
description: Recupere as propriedades e os relacionamentos de todos os objetos offerShiftRequest de uma equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 411363d06a677c6b211d85e058766923a136a505
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44153538"
---
# <a name="list-offershiftrequest"></a><span data-ttu-id="aa0c5-103">Listar offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="aa0c5-103">List offerShiftRequest</span></span>

<span data-ttu-id="aa0c5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa0c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa0c5-105">Recupere as propriedades e os relacionamentos de todos os objetos [offerShiftRequest](../resources/offershiftrequest.md) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="aa0c5-105">Retrieve the properties and relationships of all [offerShiftRequest](../resources/offershiftrequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa0c5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa0c5-106">Permissions</span></span>

<span data-ttu-id="aa0c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa0c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aa0c5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa0c5-109">Permission type</span></span>                        | <span data-ttu-id="aa0c5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa0c5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aa0c5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa0c5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aa0c5-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa0c5-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="aa0c5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa0c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa0c5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa0c5-114">Not supported.</span></span> |
| <span data-ttu-id="aa0c5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa0c5-115">Application</span></span>                            | <span data-ttu-id="aa0c5-116">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="aa0c5-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="aa0c5-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="aa0c5-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="aa0c5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa0c5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa0c5-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aa0c5-119">Optional query parameters</span></span>

<span data-ttu-id="aa0c5-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aa0c5-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="aa0c5-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="aa0c5-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa0c5-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa0c5-122">Request headers</span></span>

| <span data-ttu-id="aa0c5-123">Nome</span><span class="sxs-lookup"><span data-stu-id="aa0c5-123">Name</span></span>      |<span data-ttu-id="aa0c5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa0c5-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aa0c5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa0c5-125">Authorization</span></span> | <span data-ttu-id="aa0c5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa0c5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa0c5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa0c5-128">Request body</span></span>

<span data-ttu-id="aa0c5-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aa0c5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa0c5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa0c5-130">Response</span></span>

<span data-ttu-id="aa0c5-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [offerShiftRequest](../resources/offershiftrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa0c5-131">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aa0c5-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="aa0c5-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aa0c5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa0c5-133">Request</span></span>

<span data-ttu-id="aa0c5-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa0c5-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aa0c5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa0c5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests
```
# <a name="c"></a>[<span data-ttu-id="aa0c5-136">C#</span><span class="sxs-lookup"><span data-stu-id="aa0c5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa0c5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa0c5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa0c5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa0c5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aa0c5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa0c5-139">Response</span></span>

<span data-ttu-id="aa0c5-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aa0c5-140">The following is an example of the response.</span></span>

> <span data-ttu-id="aa0c5-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa0c5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

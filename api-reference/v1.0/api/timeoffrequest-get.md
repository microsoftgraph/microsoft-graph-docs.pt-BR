---
title: Obter timeOffRequest
description: Recupere as propriedades e as relações de um objeto timeOffRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 99683f33448c4d7b492b19f07f2f0fc704b73753
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52034389"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="2f0c8-103">Obter timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="2f0c8-103">Get timeOffRequest</span></span>

<span data-ttu-id="2f0c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f0c8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2f0c8-105">Recupere as propriedades e as relações de um [objeto timeoffrequest.](../resources/timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="2f0c8-105">Retrieve the properties and relationships of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f0c8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f0c8-106">Permissions</span></span>

<span data-ttu-id="2f0c8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f0c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f0c8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f0c8-109">Permission type</span></span>                        | <span data-ttu-id="2f0c8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f0c8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="2f0c8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f0c8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2f0c8-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f0c8-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2f0c8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f0c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f0c8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f0c8-114">Not supported.</span></span>    |
|<span data-ttu-id="2f0c8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f0c8-115">Application</span></span> | <span data-ttu-id="2f0c8-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f0c8-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="2f0c8-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="2f0c8-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2f0c8-118">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="2f0c8-118">Global admins can access groups that they are not a member of.</span></span> <span data-ttu-id="2f0c8-119">atualmente apenas em visualização privada e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="2f0c8-119">currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="2f0c8-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f0c8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f0c8-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2f0c8-121">Optional query parameters</span></span>

<span data-ttu-id="2f0c8-122">Este método não dá suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2f0c8-122">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f0c8-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f0c8-123">Request headers</span></span>

| <span data-ttu-id="2f0c8-124">Nome</span><span class="sxs-lookup"><span data-stu-id="2f0c8-124">Name</span></span>      |<span data-ttu-id="2f0c8-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f0c8-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2f0c8-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f0c8-126">Authorization</span></span> | <span data-ttu-id="2f0c8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f0c8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f0c8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f0c8-129">Request body</span></span>

<span data-ttu-id="2f0c8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f0c8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f0c8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f0c8-131">Response</span></span>

<span data-ttu-id="2f0c8-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [timeOffRequest](../resources/timeoffrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f0c8-132">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f0c8-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2f0c8-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2f0c8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f0c8-134">Request</span></span>

<span data-ttu-id="2f0c8-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f0c8-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2f0c8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f0c8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="2f0c8-137">C#</span><span class="sxs-lookup"><span data-stu-id="2f0c8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f0c8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f0c8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f0c8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f0c8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f0c8-140">Java</span><span class="sxs-lookup"><span data-stu-id="2f0c8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-timeoffrequest-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="2f0c8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f0c8-141">Response</span></span>

<span data-ttu-id="2f0c8-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f0c8-142">The following is an example of the response.</span></span>

> <span data-ttu-id="2f0c8-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2f0c8-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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


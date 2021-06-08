---
title: 'timeOffRequest: decline'
description: Recusar um objeto timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7f9e5f6151e30dbbfcfc74db51a9a8e2afacab1c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787419"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="fb973-103">timeOffRequest: decline</span><span class="sxs-lookup"><span data-stu-id="fb973-103">timeOffRequest: decline</span></span>

<span data-ttu-id="fb973-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb973-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fb973-105">Recusar um [objeto timeoffrequest.](../resources/timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="fb973-105">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb973-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb973-106">Permissions</span></span>

<span data-ttu-id="fb973-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb973-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fb973-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb973-109">Permission type</span></span>                        | <span data-ttu-id="fb973-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb973-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="fb973-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb973-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fb973-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb973-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fb973-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb973-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb973-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb973-114">Not supported.</span></span>    |
|<span data-ttu-id="fb973-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb973-115">Application</span></span> | <span data-ttu-id="fb973-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb973-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="fb973-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="fb973-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="fb973-118">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="fb973-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="fb973-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb973-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="fb973-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb973-120">Request headers</span></span>

| <span data-ttu-id="fb973-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fb973-121">Name</span></span>          | <span data-ttu-id="fb973-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb973-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fb973-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb973-123">Authorization</span></span> | <span data-ttu-id="fb973-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb973-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fb973-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="fb973-126">Content-type</span></span> | <span data-ttu-id="fb973-127">application-json.</span><span class="sxs-lookup"><span data-stu-id="fb973-127">application-json.</span></span> <span data-ttu-id="fb973-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb973-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb973-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb973-129">Request body</span></span>

<span data-ttu-id="fb973-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb973-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fb973-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fb973-131">Parameter</span></span>    | <span data-ttu-id="fb973-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb973-132">Type</span></span>        | <span data-ttu-id="fb973-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb973-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fb973-134">mensagem</span><span class="sxs-lookup"><span data-stu-id="fb973-134">message</span></span>|<span data-ttu-id="fb973-135">String</span><span class="sxs-lookup"><span data-stu-id="fb973-135">String</span></span>|<span data-ttu-id="fb973-136">Mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="fb973-136">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="fb973-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb973-137">Response</span></span>

<span data-ttu-id="fb973-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb973-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fb973-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fb973-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fb973-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb973-141">Request</span></span>

<span data-ttu-id="fb973-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb973-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fb973-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb973-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="fb973-144">C#</span><span class="sxs-lookup"><span data-stu-id="fb973-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb973-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb973-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb973-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb973-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb973-147">Java</span><span class="sxs-lookup"><span data-stu-id="fb973-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffrequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="fb973-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb973-148">Response</span></span>

<span data-ttu-id="fb973-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fb973-149">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeOffRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


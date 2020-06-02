---
title: 'timeOffRequest: recusar'
description: Recusar um objeto timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a76fd617ddb71d5ffcae0a82b716d2915143d1f6
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44217091"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="af1e4-103">timeOffRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="af1e4-103">timeOffRequest: decline</span></span>

<span data-ttu-id="af1e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af1e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af1e4-105">Recusar um objeto [timeoffrequest](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="af1e4-105">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="af1e4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="af1e4-106">Permissions</span></span>

<span data-ttu-id="af1e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af1e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="af1e4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af1e4-109">Permission type</span></span>                        | <span data-ttu-id="af1e4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af1e4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="af1e4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af1e4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="af1e4-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af1e4-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="af1e4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af1e4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af1e4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af1e4-114">Not supported.</span></span> |
|<span data-ttu-id="af1e4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af1e4-115">Application</span></span> | <span data-ttu-id="af1e4-116">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="af1e4-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="af1e4-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="af1e4-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="af1e4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af1e4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="af1e4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af1e4-119">Request headers</span></span>

| <span data-ttu-id="af1e4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="af1e4-120">Name</span></span>          | <span data-ttu-id="af1e4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="af1e4-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="af1e4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="af1e4-122">Authorization</span></span> | <span data-ttu-id="af1e4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af1e4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="af1e4-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="af1e4-125">Content-type</span></span> | <span data-ttu-id="af1e4-126">Application-JSON.</span><span class="sxs-lookup"><span data-stu-id="af1e4-126">application-json.</span></span> <span data-ttu-id="af1e4-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af1e4-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="af1e4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af1e4-128">Request body</span></span>

<span data-ttu-id="af1e4-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af1e4-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="af1e4-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="af1e4-130">Parameter</span></span>    | <span data-ttu-id="af1e4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="af1e4-131">Type</span></span>        | <span data-ttu-id="af1e4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="af1e4-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="af1e4-133">mensagem</span><span class="sxs-lookup"><span data-stu-id="af1e4-133">message</span></span>|<span data-ttu-id="af1e4-134">String</span><span class="sxs-lookup"><span data-stu-id="af1e4-134">String</span></span>|<span data-ttu-id="af1e4-135">Mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="af1e4-135">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="af1e4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="af1e4-136">Response</span></span>

<span data-ttu-id="af1e4-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af1e4-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="af1e4-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="af1e4-139">Examples</span></span>

<span data-ttu-id="af1e4-140">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="af1e4-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="af1e4-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af1e4-141">Request</span></span>

<span data-ttu-id="af1e4-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="af1e4-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="af1e4-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="af1e4-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="javascript"></a>[<span data-ttu-id="af1e4-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af1e4-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af1e4-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af1e4-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="af1e4-146">C#</span><span class="sxs-lookup"><span data-stu-id="af1e4-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="af1e4-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="af1e4-147">Response</span></span>

<span data-ttu-id="af1e4-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="af1e4-148">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
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

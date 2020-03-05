---
title: 'timeOffRequest: recusar'
description: Recusar um objeto timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9b99949d8ae30d208e1d1939c6473c8767d6cbd6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452257"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="db4c0-103">timeOffRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="db4c0-103">timeOffRequest: decline</span></span>

<span data-ttu-id="db4c0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="db4c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db4c0-105">Recusar um objeto [timeoffrequest](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="db4c0-105">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="db4c0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="db4c0-106">Permissions</span></span>

<span data-ttu-id="db4c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db4c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db4c0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db4c0-109">Permission type</span></span>                        | <span data-ttu-id="db4c0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db4c0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="db4c0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db4c0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="db4c0-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db4c0-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="db4c0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db4c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db4c0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db4c0-114">Not supported.</span></span> |
|<span data-ttu-id="db4c0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db4c0-115">Application</span></span> | <span data-ttu-id="db4c0-116">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="db4c0-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="db4c0-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="db4c0-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="db4c0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db4c0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/timeOffRequests/decline
```

## <a name="request-headers"></a><span data-ttu-id="db4c0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db4c0-119">Request headers</span></span>

| <span data-ttu-id="db4c0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="db4c0-120">Name</span></span>          | <span data-ttu-id="db4c0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="db4c0-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="db4c0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="db4c0-122">Authorization</span></span> | <span data-ttu-id="db4c0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db4c0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db4c0-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="db4c0-125">Content-type</span></span> | <span data-ttu-id="db4c0-126">Application-JSON.</span><span class="sxs-lookup"><span data-stu-id="db4c0-126">application-json.</span></span> <span data-ttu-id="db4c0-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db4c0-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db4c0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db4c0-128">Request body</span></span>

<span data-ttu-id="db4c0-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db4c0-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="db4c0-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="db4c0-130">Parameter</span></span>    | <span data-ttu-id="db4c0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="db4c0-131">Type</span></span>        | <span data-ttu-id="db4c0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="db4c0-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="db4c0-133">mensagem</span><span class="sxs-lookup"><span data-stu-id="db4c0-133">message</span></span>|<span data-ttu-id="db4c0-134">String</span><span class="sxs-lookup"><span data-stu-id="db4c0-134">String</span></span>|<span data-ttu-id="db4c0-135">Mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="db4c0-135">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="db4c0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="db4c0-136">Response</span></span>

<span data-ttu-id="db4c0-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db4c0-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db4c0-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="db4c0-139">Examples</span></span>

<span data-ttu-id="db4c0-140">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="db4c0-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="db4c0-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db4c0-141">Request</span></span>

<span data-ttu-id="db4c0-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db4c0-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db4c0-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="db4c0-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="javascript"></a>[<span data-ttu-id="db4c0-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db4c0-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db4c0-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db4c0-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="db4c0-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="db4c0-146">Response</span></span>

<span data-ttu-id="db4c0-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db4c0-147">The following is an example of the response.</span></span>
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

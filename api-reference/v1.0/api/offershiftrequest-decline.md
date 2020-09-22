---
title: 'offerShiftRequest: recusar'
description: Recusar uma solicitação de mudança de oferta.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8368935da77d178c7e1165da4b9ac418a9016f0e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087142"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="cc6dc-103">offerShiftRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="cc6dc-103">offerShiftRequest: decline</span></span>

<span data-ttu-id="cc6dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc6dc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc6dc-105">Recusar um objeto [offerShiftRequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="cc6dc-105">Decline an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc6dc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc6dc-106">Permissions</span></span>

<span data-ttu-id="cc6dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc6dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc6dc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc6dc-109">Permission type</span></span>                        | <span data-ttu-id="cc6dc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc6dc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cc6dc-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc6dc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc6dc-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cc6dc-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="cc6dc-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc6dc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc6dc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc6dc-114">Not supported.</span></span> |
| <span data-ttu-id="cc6dc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc6dc-115">Application</span></span>                            | <span data-ttu-id="cc6dc-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc6dc-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="cc6dc-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="cc6dc-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="cc6dc-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="cc6dc-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cc6dc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc6dc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="cc6dc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc6dc-120">Request headers</span></span>

| <span data-ttu-id="cc6dc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="cc6dc-121">Name</span></span>          | <span data-ttu-id="cc6dc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc6dc-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cc6dc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc6dc-123">Authorization</span></span> | <span data-ttu-id="cc6dc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc6dc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cc6dc-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="cc6dc-126">Content-type</span></span> | <span data-ttu-id="cc6dc-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc6dc-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc6dc-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc6dc-129">Request body</span></span>

<span data-ttu-id="cc6dc-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc6dc-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cc6dc-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cc6dc-131">Parameter</span></span>    | <span data-ttu-id="cc6dc-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc6dc-132">Type</span></span>        | <span data-ttu-id="cc6dc-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc6dc-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cc6dc-134">mensagem</span><span class="sxs-lookup"><span data-stu-id="cc6dc-134">message</span></span>|<span data-ttu-id="cc6dc-135">String</span><span class="sxs-lookup"><span data-stu-id="cc6dc-135">String</span></span>|<span data-ttu-id="cc6dc-136">Mensagem personalizada enviada ao recusar.</span><span class="sxs-lookup"><span data-stu-id="cc6dc-136">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="cc6dc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc6dc-137">Response</span></span>

<span data-ttu-id="cc6dc-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc6dc-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc6dc-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cc6dc-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cc6dc-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc6dc-141">Request</span></span>

<span data-ttu-id="cc6dc-142">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc6dc-142">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cc6dc-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc6dc-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
Content-type: application/json

{
  "message": "Sorry, you can't offer this shift."
}
```
# <a name="c"></a>[<span data-ttu-id="cc6dc-144">C#</span><span class="sxs-lookup"><span data-stu-id="cc6dc-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc6dc-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc6dc-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc6dc-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc6dc-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc6dc-147">Java</span><span class="sxs-lookup"><span data-stu-id="cc6dc-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/offershiftrequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="cc6dc-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc6dc-148">Response</span></span>

<span data-ttu-id="cc6dc-149">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="cc6dc-149">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


---
title: 'openShiftChangeRequest: decline'
description: Recusar uma solicitação de abertura.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 480987fdc6e9b1dc9d3c52bfd47d3737928dff40
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447856"
---
# <a name="openshiftchangerequest-decline"></a><span data-ttu-id="d7653-103">openShiftChangeRequest: decline</span><span class="sxs-lookup"><span data-stu-id="d7653-103">openShiftChangeRequest: decline</span></span>

<span data-ttu-id="d7653-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7653-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7653-105">Recusar um [objeto openshiftchangerequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="d7653-105">Decline an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7653-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7653-106">Permissions</span></span>

<span data-ttu-id="d7653-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7653-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7653-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7653-109">Permission type</span></span>                        | <span data-ttu-id="d7653-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d7653-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d7653-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7653-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7653-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7653-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d7653-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7653-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7653-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7653-114">Not supported.</span></span> |
| <span data-ttu-id="d7653-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7653-115">Application</span></span>                            | <span data-ttu-id="d7653-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7653-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7653-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7653-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="d7653-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7653-118">Request headers</span></span>

| <span data-ttu-id="d7653-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d7653-119">Name</span></span>          | <span data-ttu-id="d7653-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7653-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d7653-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7653-121">Authorization</span></span> | <span data-ttu-id="d7653-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7653-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7653-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7653-124">Request body</span></span>

<span data-ttu-id="d7653-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7653-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d7653-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d7653-126">Parameter</span></span>    | <span data-ttu-id="d7653-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7653-127">Type</span></span>        | <span data-ttu-id="d7653-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7653-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d7653-129">mensagem</span><span class="sxs-lookup"><span data-stu-id="d7653-129">message</span></span>|<span data-ttu-id="d7653-130">String</span><span class="sxs-lookup"><span data-stu-id="d7653-130">String</span></span>|<span data-ttu-id="d7653-131">Uma mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="d7653-131">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="d7653-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7653-132">Response</span></span>

<span data-ttu-id="d7653-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7653-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d7653-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d7653-135">Examples</span></span>

<span data-ttu-id="d7653-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d7653-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d7653-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7653-137">Request</span></span>

<span data-ttu-id="d7653-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7653-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d7653-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7653-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d7653-140">C#</span><span class="sxs-lookup"><span data-stu-id="d7653-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/openshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7653-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7653-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/openshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7653-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7653-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/openshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7653-143">Java</span><span class="sxs-lookup"><span data-stu-id="d7653-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/openshiftchangerequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d7653-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7653-144">Response</span></span>

<span data-ttu-id="d7653-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d7653-145">The following is an example of the response.</span></span>
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
  "description": "openShiftChangeRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



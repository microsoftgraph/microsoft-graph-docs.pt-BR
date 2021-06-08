---
title: 'openShiftChangeRequest: decline'
description: Recusar uma solicitação de abertura.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 64a54cba75b1f71e4bce43ca8bced4e2bb5841e8
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785939"
---
# <a name="openshiftchangerequest-decline"></a><span data-ttu-id="39cc9-103">openShiftChangeRequest: decline</span><span class="sxs-lookup"><span data-stu-id="39cc9-103">openShiftChangeRequest: decline</span></span>

<span data-ttu-id="39cc9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39cc9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39cc9-105">Recusar um [objeto openshiftchangerequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="39cc9-105">Decline an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="39cc9-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="39cc9-106">Permissions</span></span>

<span data-ttu-id="39cc9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39cc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="39cc9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39cc9-109">Permission type</span></span>                        | <span data-ttu-id="39cc9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39cc9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="39cc9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39cc9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="39cc9-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39cc9-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="39cc9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39cc9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39cc9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39cc9-114">Not supported.</span></span> |
| <span data-ttu-id="39cc9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39cc9-115">Application</span></span>                            | <span data-ttu-id="39cc9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39cc9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39cc9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39cc9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="39cc9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39cc9-118">Request headers</span></span>

| <span data-ttu-id="39cc9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="39cc9-119">Name</span></span>          | <span data-ttu-id="39cc9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="39cc9-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="39cc9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="39cc9-121">Authorization</span></span> | <span data-ttu-id="39cc9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39cc9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39cc9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39cc9-124">Request body</span></span>

<span data-ttu-id="39cc9-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39cc9-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="39cc9-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="39cc9-126">Parameter</span></span>    | <span data-ttu-id="39cc9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="39cc9-127">Type</span></span>        | <span data-ttu-id="39cc9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="39cc9-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="39cc9-129">mensagem</span><span class="sxs-lookup"><span data-stu-id="39cc9-129">message</span></span>|<span data-ttu-id="39cc9-130">String</span><span class="sxs-lookup"><span data-stu-id="39cc9-130">String</span></span>|<span data-ttu-id="39cc9-131">Uma mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="39cc9-131">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="39cc9-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="39cc9-132">Response</span></span>

<span data-ttu-id="39cc9-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39cc9-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="39cc9-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="39cc9-135">Examples</span></span>

<span data-ttu-id="39cc9-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="39cc9-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="39cc9-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39cc9-137">Request</span></span>

<span data-ttu-id="39cc9-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="39cc9-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39cc9-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="39cc9-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="39cc9-140">C#</span><span class="sxs-lookup"><span data-stu-id="39cc9-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/openshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39cc9-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39cc9-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/openshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39cc9-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39cc9-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/openshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39cc9-143">Java</span><span class="sxs-lookup"><span data-stu-id="39cc9-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/openshiftchangerequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="39cc9-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="39cc9-144">Response</span></span>

<span data-ttu-id="39cc9-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="39cc9-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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



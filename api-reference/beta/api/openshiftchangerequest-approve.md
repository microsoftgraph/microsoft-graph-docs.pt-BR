---
title: 'openShiftChangeRequest: aprovar'
description: Aprovar uma solicitação de abertura.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a6ce178eb59045d572bed00d790c2405be349e5a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447869"
---
# <a name="openshiftchangerequest-approve"></a><span data-ttu-id="1996d-103">openShiftChangeRequest: aprovar</span><span class="sxs-lookup"><span data-stu-id="1996d-103">openShiftChangeRequest: approve</span></span>

<span data-ttu-id="1996d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1996d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1996d-105">Aprovar um [objeto openshiftchangerequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="1996d-105">Approve an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1996d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1996d-106">Permissions</span></span>

<span data-ttu-id="1996d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1996d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1996d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1996d-109">Permission type</span></span>                        | <span data-ttu-id="1996d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1996d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1996d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1996d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1996d-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1996d-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1996d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1996d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1996d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1996d-114">Not supported.</span></span> |
| <span data-ttu-id="1996d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1996d-115">Application</span></span>                            | <span data-ttu-id="1996d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1996d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1996d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1996d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="1996d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1996d-118">Request headers</span></span>

| <span data-ttu-id="1996d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1996d-119">Name</span></span>          | <span data-ttu-id="1996d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1996d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1996d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1996d-121">Authorization</span></span> | <span data-ttu-id="1996d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1996d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1996d-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="1996d-124">Content-type</span></span> | <span data-ttu-id="1996d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1996d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1996d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1996d-127">Request body</span></span>

<span data-ttu-id="1996d-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1996d-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1996d-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1996d-129">Parameter</span></span>    | <span data-ttu-id="1996d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1996d-130">Type</span></span>        | <span data-ttu-id="1996d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1996d-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1996d-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="1996d-132">message</span></span>|<span data-ttu-id="1996d-133">String</span><span class="sxs-lookup"><span data-stu-id="1996d-133">String</span></span>|<span data-ttu-id="1996d-134">Uma mensagem de aprovação personalizada.</span><span class="sxs-lookup"><span data-stu-id="1996d-134">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="1996d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1996d-135">Response</span></span>

<span data-ttu-id="1996d-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1996d-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1996d-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1996d-138">Examples</span></span>

<span data-ttu-id="1996d-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="1996d-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1996d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1996d-140">Request</span></span>

<span data-ttu-id="1996d-141">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="1996d-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1996d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="1996d-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="1996d-143">C#</span><span class="sxs-lookup"><span data-stu-id="1996d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/openshiftchangerequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1996d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1996d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/openshiftchangerequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1996d-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1996d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/openshiftchangerequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1996d-146">Java</span><span class="sxs-lookup"><span data-stu-id="1996d-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/openshiftchangerequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1996d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="1996d-147">Response</span></span>

<span data-ttu-id="1996d-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1996d-148">The following is an example of the response.</span></span>
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
  "description": "openShiftChangeRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



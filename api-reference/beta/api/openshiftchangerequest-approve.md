---
title: 'openShiftChangeRequest: aprovar'
description: Aprovar uma solicitação de abertura.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 769665c9a65229d33e287fcf7660157c5aa0b425
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785947"
---
# <a name="openshiftchangerequest-approve"></a><span data-ttu-id="1e5c2-103">openShiftChangeRequest: aprovar</span><span class="sxs-lookup"><span data-stu-id="1e5c2-103">openShiftChangeRequest: approve</span></span>

<span data-ttu-id="1e5c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e5c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e5c2-105">Aprovar um [objeto openshiftchangerequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="1e5c2-105">Approve an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e5c2-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="1e5c2-106">Permissions</span></span>

<span data-ttu-id="1e5c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e5c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1e5c2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e5c2-109">Permission type</span></span>                        | <span data-ttu-id="1e5c2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e5c2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1e5c2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e5c2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1e5c2-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e5c2-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1e5c2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e5c2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e5c2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e5c2-114">Not supported.</span></span> |
| <span data-ttu-id="1e5c2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e5c2-115">Application</span></span>                            | <span data-ttu-id="1e5c2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e5c2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e5c2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e5c2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="1e5c2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e5c2-118">Request headers</span></span>

| <span data-ttu-id="1e5c2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1e5c2-119">Name</span></span>          | <span data-ttu-id="1e5c2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e5c2-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1e5c2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e5c2-121">Authorization</span></span> | <span data-ttu-id="1e5c2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e5c2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1e5c2-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="1e5c2-124">Content-type</span></span> | <span data-ttu-id="1e5c2-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e5c2-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e5c2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e5c2-127">Request body</span></span>

<span data-ttu-id="1e5c2-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e5c2-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1e5c2-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1e5c2-129">Parameter</span></span>    | <span data-ttu-id="1e5c2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e5c2-130">Type</span></span>        | <span data-ttu-id="1e5c2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e5c2-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1e5c2-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="1e5c2-132">message</span></span>|<span data-ttu-id="1e5c2-133">String</span><span class="sxs-lookup"><span data-stu-id="1e5c2-133">String</span></span>|<span data-ttu-id="1e5c2-134">Uma mensagem de aprovação personalizada.</span><span class="sxs-lookup"><span data-stu-id="1e5c2-134">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="1e5c2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e5c2-135">Response</span></span>

<span data-ttu-id="1e5c2-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e5c2-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1e5c2-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1e5c2-138">Examples</span></span>

<span data-ttu-id="1e5c2-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="1e5c2-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1e5c2-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e5c2-140">Request</span></span>

<span data-ttu-id="1e5c2-141">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e5c2-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1e5c2-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e5c2-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1e5c2-143">C#</span><span class="sxs-lookup"><span data-stu-id="1e5c2-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/openshiftchangerequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1e5c2-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e5c2-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/openshiftchangerequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1e5c2-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e5c2-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/openshiftchangerequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1e5c2-146">Java</span><span class="sxs-lookup"><span data-stu-id="1e5c2-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/openshiftchangerequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1e5c2-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e5c2-147">Response</span></span>

<span data-ttu-id="1e5c2-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1e5c2-148">The following is an example of the response.</span></span>
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
  "description": "openShiftChangeRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



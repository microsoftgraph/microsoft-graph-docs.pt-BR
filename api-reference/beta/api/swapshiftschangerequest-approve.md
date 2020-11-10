---
title: 'swapShiftsChangeRequest: aprovar'
description: Aprovar uma solicitação Shift de troca.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 56dd5e9696bc32cfa48eeaf1a19f2d228de93c38
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982158"
---
# <a name="swapshiftschangerequest-approve"></a><span data-ttu-id="9db16-103">swapShiftsChangeRequest: aprovar</span><span class="sxs-lookup"><span data-stu-id="9db16-103">swapShiftsChangeRequest: approve</span></span>

<span data-ttu-id="9db16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9db16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9db16-105">Aprovar um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="9db16-105">Approve a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9db16-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9db16-106">Permissions</span></span>

<span data-ttu-id="9db16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9db16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9db16-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9db16-109">Permission type</span></span>                        | <span data-ttu-id="9db16-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9db16-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9db16-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9db16-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9db16-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9db16-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="9db16-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9db16-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9db16-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9db16-114">Not supported.</span></span> |
| <span data-ttu-id="9db16-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9db16-115">Application</span></span>                            | <span data-ttu-id="9db16-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9db16-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9db16-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9db16-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="9db16-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9db16-118">Request headers</span></span>

| <span data-ttu-id="9db16-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9db16-119">Name</span></span>          | <span data-ttu-id="9db16-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9db16-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9db16-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9db16-121">Authorization</span></span> | <span data-ttu-id="9db16-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9db16-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9db16-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="9db16-124">Content-type</span></span> | <span data-ttu-id="9db16-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9db16-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9db16-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9db16-127">Request body</span></span>

<span data-ttu-id="9db16-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9db16-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9db16-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9db16-129">Parameter</span></span>    | <span data-ttu-id="9db16-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9db16-130">Type</span></span>        | <span data-ttu-id="9db16-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9db16-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9db16-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="9db16-132">message</span></span>|<span data-ttu-id="9db16-133">String</span><span class="sxs-lookup"><span data-stu-id="9db16-133">String</span></span>|<span data-ttu-id="9db16-134">Uma mensagem de aprovação personalizada.</span><span class="sxs-lookup"><span data-stu-id="9db16-134">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="9db16-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9db16-135">Response</span></span>

<span data-ttu-id="9db16-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9db16-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9db16-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9db16-138">Examples</span></span>

<span data-ttu-id="9db16-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="9db16-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="9db16-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9db16-140">Request</span></span>

<span data-ttu-id="9db16-141">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="9db16-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9db16-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="9db16-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="9db16-143">C#</span><span class="sxs-lookup"><span data-stu-id="9db16-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9db16-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9db16-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9db16-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9db16-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9db16-146">Java</span><span class="sxs-lookup"><span data-stu-id="9db16-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/swapshiftchangerequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9db16-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="9db16-147">Response</span></span>

<span data-ttu-id="9db16-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9db16-148">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftChangeRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



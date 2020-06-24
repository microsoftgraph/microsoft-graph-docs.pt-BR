---
title: 'swapShiftsChangeRequest: recusar'
description: Recusar uma solicitação Shift de troca.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4814fb3ef9d416d6d3bc5be1815b746277a25426
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846181"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="6a8cb-103">swapShiftsChangeRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="6a8cb-103">swapShiftsChangeRequest: decline</span></span>

<span data-ttu-id="6a8cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a8cb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6a8cb-105">Recusar um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="6a8cb-105">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a8cb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a8cb-106">Permissions</span></span>

<span data-ttu-id="6a8cb-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6a8cb-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6a8cb-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a8cb-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a8cb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a8cb-109">Permission type</span></span>                        | <span data-ttu-id="6a8cb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a8cb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6a8cb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a8cb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a8cb-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6a8cb-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="6a8cb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a8cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a8cb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a8cb-114">Not supported.</span></span>                              |
| <span data-ttu-id="6a8cb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a8cb-115">Application</span></span>                            | <span data-ttu-id="6a8cb-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8cb-116">Schedule.ReadWrite.All</span></span>                      |

> <span data-ttu-id="6a8cb-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="6a8cb-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6a8cb-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="6a8cb-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6a8cb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a8cb-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="6a8cb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a8cb-120">Request headers</span></span>

| <span data-ttu-id="6a8cb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6a8cb-121">Name</span></span>          | <span data-ttu-id="6a8cb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a8cb-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6a8cb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a8cb-123">Authorization</span></span> | <span data-ttu-id="6a8cb-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="6a8cb-124">Bearer {token}.</span></span> <span data-ttu-id="6a8cb-125">Required.</span><span class="sxs-lookup"><span data-stu-id="6a8cb-125">Required.</span></span> |
| <span data-ttu-id="6a8cb-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="6a8cb-126">Content-type</span></span> | <span data-ttu-id="6a8cb-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="6a8cb-127">application/json.</span></span> <span data-ttu-id="6a8cb-128">Required.</span><span class="sxs-lookup"><span data-stu-id="6a8cb-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a8cb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a8cb-129">Request body</span></span>

<span data-ttu-id="6a8cb-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a8cb-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6a8cb-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6a8cb-131">Parameter</span></span>    | <span data-ttu-id="6a8cb-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a8cb-132">Type</span></span>        | <span data-ttu-id="6a8cb-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a8cb-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6a8cb-134">mensagem</span><span class="sxs-lookup"><span data-stu-id="6a8cb-134">message</span></span>|<span data-ttu-id="6a8cb-135">String</span><span class="sxs-lookup"><span data-stu-id="6a8cb-135">String</span></span>|<span data-ttu-id="6a8cb-136">Uma mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="6a8cb-136">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="6a8cb-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a8cb-137">Response</span></span>

<span data-ttu-id="6a8cb-138">If successful, this method returns a `200 OK` response code.</span><span class="sxs-lookup"><span data-stu-id="6a8cb-138">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="6a8cb-139">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="6a8cb-139">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a8cb-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6a8cb-140">Examples</span></span>

<span data-ttu-id="6a8cb-141">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="6a8cb-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6a8cb-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a8cb-142">Request</span></span>

<span data-ttu-id="6a8cb-143">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a8cb-143">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6a8cb-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a8cb-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="6a8cb-145">C#</span><span class="sxs-lookup"><span data-stu-id="6a8cb-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a8cb-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a8cb-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a8cb-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a8cb-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a8cb-148">Java</span><span class="sxs-lookup"><span data-stu-id="6a8cb-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/swapshiftchangerequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="6a8cb-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a8cb-149">Response</span></span>

<span data-ttu-id="6a8cb-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6a8cb-150">The following is an example of the response.</span></span>
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
  "description": "swapShiftChangeRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

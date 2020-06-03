---
title: 'swapShiftsChangeRequest: recusar'
description: Recusar uma solicitação Shift de troca.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d2b53c049dfb1213fdae049e0d8f1cb72b6a1f95
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44217451"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="19bd7-103">swapShiftsChangeRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="19bd7-103">swapShiftsChangeRequest: decline</span></span>

<span data-ttu-id="19bd7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19bd7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19bd7-105">Recusar um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="19bd7-105">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="19bd7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="19bd7-106">Permissions</span></span>

<span data-ttu-id="19bd7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19bd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19bd7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19bd7-109">Permission type</span></span>                        | <span data-ttu-id="19bd7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19bd7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="19bd7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19bd7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="19bd7-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="19bd7-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="19bd7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19bd7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19bd7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19bd7-114">Not supported.</span></span>    |<span data-ttu-id="19bd7-115">s</span><span class="sxs-lookup"><span data-stu-id="19bd7-115">s</span></span>
|<span data-ttu-id="19bd7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19bd7-116">Application</span></span> | <span data-ttu-id="19bd7-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19bd7-117">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="19bd7-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="19bd7-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="19bd7-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="19bd7-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="19bd7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19bd7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="19bd7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19bd7-121">Request headers</span></span>

| <span data-ttu-id="19bd7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="19bd7-122">Name</span></span>          | <span data-ttu-id="19bd7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="19bd7-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="19bd7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="19bd7-124">Authorization</span></span> | <span data-ttu-id="19bd7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19bd7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19bd7-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="19bd7-127">Content-type</span></span> | <span data-ttu-id="19bd7-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19bd7-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19bd7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19bd7-130">Request body</span></span>

<span data-ttu-id="19bd7-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19bd7-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="19bd7-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="19bd7-132">Parameter</span></span>    | <span data-ttu-id="19bd7-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="19bd7-133">Type</span></span>        | <span data-ttu-id="19bd7-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="19bd7-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="19bd7-135">mensagem</span><span class="sxs-lookup"><span data-stu-id="19bd7-135">message</span></span>|<span data-ttu-id="19bd7-136">String</span><span class="sxs-lookup"><span data-stu-id="19bd7-136">String</span></span>|<span data-ttu-id="19bd7-137">Uma mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="19bd7-137">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="19bd7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="19bd7-138">Response</span></span>

<span data-ttu-id="19bd7-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19bd7-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19bd7-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="19bd7-141">Examples</span></span>

<span data-ttu-id="19bd7-142">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="19bd7-142">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="19bd7-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19bd7-143">Request</span></span>

<span data-ttu-id="19bd7-144">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="19bd7-144">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="19bd7-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="19bd7-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="19bd7-146">C#</span><span class="sxs-lookup"><span data-stu-id="19bd7-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19bd7-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19bd7-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19bd7-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19bd7-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="19bd7-149">Java</span><span class="sxs-lookup"><span data-stu-id="19bd7-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/swapshiftchangerequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="19bd7-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="19bd7-150">Response</span></span>

<span data-ttu-id="19bd7-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19bd7-151">The following is an example of the response.</span></span>
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

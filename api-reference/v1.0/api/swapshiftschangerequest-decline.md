---
title: 'swapShiftsChangeRequest: recusar'
description: Recusar uma solicitação Shift de troca.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d32f712485315ef82efeb3777559ac4d472ed59b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984562"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="b9f04-103">swapShiftsChangeRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="b9f04-103">swapShiftsChangeRequest: decline</span></span>

<span data-ttu-id="b9f04-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9f04-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9f04-105">Recusar um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="b9f04-105">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9f04-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9f04-106">Permissions</span></span>

<span data-ttu-id="b9f04-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9f04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9f04-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9f04-109">Permission type</span></span>                        | <span data-ttu-id="b9f04-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9f04-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b9f04-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9f04-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9f04-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b9f04-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="b9f04-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9f04-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9f04-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9f04-114">Not supported.</span></span>                              |
| <span data-ttu-id="b9f04-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9f04-115">Application</span></span>                            | <span data-ttu-id="b9f04-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9f04-116">Schedule.ReadWrite.All</span></span>                      |

> <span data-ttu-id="b9f04-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="b9f04-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b9f04-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="b9f04-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b9f04-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9f04-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="b9f04-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9f04-120">Request headers</span></span>

| <span data-ttu-id="b9f04-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b9f04-121">Name</span></span>          | <span data-ttu-id="b9f04-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9f04-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b9f04-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9f04-123">Authorization</span></span> | <span data-ttu-id="b9f04-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9f04-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9f04-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="b9f04-126">Content-type</span></span> | <span data-ttu-id="b9f04-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9f04-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9f04-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9f04-129">Request body</span></span>

<span data-ttu-id="b9f04-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9f04-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9f04-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b9f04-131">Parameter</span></span>    | <span data-ttu-id="b9f04-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9f04-132">Type</span></span>        | <span data-ttu-id="b9f04-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9f04-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b9f04-134">mensagem</span><span class="sxs-lookup"><span data-stu-id="b9f04-134">message</span></span>|<span data-ttu-id="b9f04-135">String</span><span class="sxs-lookup"><span data-stu-id="b9f04-135">String</span></span>|<span data-ttu-id="b9f04-136">Uma mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="b9f04-136">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="b9f04-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9f04-137">Response</span></span>

<span data-ttu-id="b9f04-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9f04-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9f04-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b9f04-140">Examples</span></span>

<span data-ttu-id="b9f04-141">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b9f04-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b9f04-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9f04-142">Request</span></span>

<span data-ttu-id="b9f04-143">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9f04-143">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b9f04-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9f04-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b9f04-145">C#</span><span class="sxs-lookup"><span data-stu-id="b9f04-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9f04-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9f04-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9f04-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9f04-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9f04-148">Java</span><span class="sxs-lookup"><span data-stu-id="b9f04-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/swapshiftchangerequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="b9f04-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9f04-149">Response</span></span>

<span data-ttu-id="b9f04-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b9f04-150">The following is an example of the response.</span></span>
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


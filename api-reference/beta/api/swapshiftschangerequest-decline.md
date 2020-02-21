---
title: 'swapShiftsChangeRequest: recusar'
description: Recusar uma solicitação Shift de troca.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 35d7d9d83dc32d7598815ed8d98e7f6f828d8b1f
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219787"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="36fc6-103">swapShiftsChangeRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="36fc6-103">swapShiftsChangeRequest: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36fc6-104">Recusar um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="36fc6-104">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="36fc6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="36fc6-105">Permissions</span></span>

<span data-ttu-id="36fc6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36fc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36fc6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36fc6-108">Permission type</span></span>                        | <span data-ttu-id="36fc6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36fc6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="36fc6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36fc6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="36fc6-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36fc6-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="36fc6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36fc6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36fc6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36fc6-113">Not supported.</span></span> |
| <span data-ttu-id="36fc6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36fc6-114">Application</span></span>                            | <span data-ttu-id="36fc6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36fc6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36fc6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36fc6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="36fc6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36fc6-117">Request headers</span></span>

| <span data-ttu-id="36fc6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="36fc6-118">Name</span></span>          | <span data-ttu-id="36fc6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="36fc6-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="36fc6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="36fc6-120">Authorization</span></span> | <span data-ttu-id="36fc6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36fc6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36fc6-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="36fc6-123">Content-type</span></span> | <span data-ttu-id="36fc6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36fc6-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36fc6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36fc6-126">Request body</span></span>

<span data-ttu-id="36fc6-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36fc6-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="36fc6-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="36fc6-128">Parameter</span></span>    | <span data-ttu-id="36fc6-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="36fc6-129">Type</span></span>        | <span data-ttu-id="36fc6-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="36fc6-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="36fc6-131">mensagem</span><span class="sxs-lookup"><span data-stu-id="36fc6-131">message</span></span>|<span data-ttu-id="36fc6-132">String</span><span class="sxs-lookup"><span data-stu-id="36fc6-132">String</span></span>|<span data-ttu-id="36fc6-133">Uma mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="36fc6-133">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="36fc6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="36fc6-134">Response</span></span>

<span data-ttu-id="36fc6-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36fc6-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36fc6-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="36fc6-137">Examples</span></span>

<span data-ttu-id="36fc6-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="36fc6-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="36fc6-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36fc6-139">Request</span></span>

<span data-ttu-id="36fc6-140">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="36fc6-140">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="36fc6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="36fc6-141">Response</span></span>

<span data-ttu-id="36fc6-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36fc6-142">The following is an example of the response.</span></span>
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

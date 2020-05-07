---
title: 'swapShiftsChangeRequest: recusar'
description: Recusar uma solicitação Shift de troca.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4f51496f69e4c49f5df4e6ccbec5cad044a79678
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154462"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="33c38-103">swapShiftsChangeRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="33c38-103">swapShiftsChangeRequest: decline</span></span>

<span data-ttu-id="33c38-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33c38-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33c38-105">Recusar um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="33c38-105">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="33c38-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="33c38-106">Permissions</span></span>

<span data-ttu-id="33c38-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33c38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="33c38-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33c38-109">Permission type</span></span>                        | <span data-ttu-id="33c38-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33c38-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="33c38-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33c38-111">Delegated (work or school account)</span></span> | <span data-ttu-id="33c38-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="33c38-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="33c38-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33c38-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33c38-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33c38-114">Not supported.</span></span>    |<span data-ttu-id="33c38-115">s</span><span class="sxs-lookup"><span data-stu-id="33c38-115">s</span></span>
|<span data-ttu-id="33c38-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33c38-116">Application</span></span> | <span data-ttu-id="33c38-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33c38-117">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="33c38-118">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="33c38-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="33c38-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="33c38-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="33c38-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33c38-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="33c38-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33c38-121">Request headers</span></span>

| <span data-ttu-id="33c38-122">Nome</span><span class="sxs-lookup"><span data-stu-id="33c38-122">Name</span></span>          | <span data-ttu-id="33c38-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="33c38-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="33c38-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="33c38-124">Authorization</span></span> | <span data-ttu-id="33c38-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33c38-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33c38-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="33c38-127">Content-type</span></span> | <span data-ttu-id="33c38-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33c38-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33c38-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33c38-130">Request body</span></span>

<span data-ttu-id="33c38-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33c38-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="33c38-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="33c38-132">Parameter</span></span>    | <span data-ttu-id="33c38-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="33c38-133">Type</span></span>        | <span data-ttu-id="33c38-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="33c38-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="33c38-135">mensagem</span><span class="sxs-lookup"><span data-stu-id="33c38-135">message</span></span>|<span data-ttu-id="33c38-136">String</span><span class="sxs-lookup"><span data-stu-id="33c38-136">String</span></span>|<span data-ttu-id="33c38-137">Uma mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="33c38-137">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="33c38-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="33c38-138">Response</span></span>

<span data-ttu-id="33c38-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33c38-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="33c38-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="33c38-141">Examples</span></span>

<span data-ttu-id="33c38-142">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="33c38-142">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="33c38-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33c38-143">Request</span></span>

<span data-ttu-id="33c38-144">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="33c38-144">The following is an example of a request.</span></span>

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
---


### <a name="response"></a><span data-ttu-id="33c38-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="33c38-145">Response</span></span>

<span data-ttu-id="33c38-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="33c38-146">The following is an example of the response.</span></span>
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

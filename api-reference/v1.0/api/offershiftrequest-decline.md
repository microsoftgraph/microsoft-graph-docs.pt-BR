---
title: 'offerShiftRequest: recusar'
description: Recusar uma solicitação de mudança de oferta.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 94daed01b2b7d4131a09504773c5377889b7e587
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154939"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="c7a1c-103">offerShiftRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="c7a1c-103">offerShiftRequest: decline</span></span>

<span data-ttu-id="c7a1c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7a1c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7a1c-105">Recusar um objeto [offerShiftRequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="c7a1c-105">Decline an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7a1c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7a1c-106">Permissions</span></span>

<span data-ttu-id="c7a1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7a1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7a1c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7a1c-109">Permission type</span></span>                        | <span data-ttu-id="c7a1c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7a1c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c7a1c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7a1c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7a1c-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c7a1c-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c7a1c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7a1c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7a1c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7a1c-114">Not supported.</span></span> |
| <span data-ttu-id="c7a1c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7a1c-115">Application</span></span>                            | <span data-ttu-id="c7a1c-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7a1c-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="c7a1c-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="c7a1c-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c7a1c-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="c7a1c-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c7a1c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7a1c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="c7a1c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7a1c-120">Request headers</span></span>

| <span data-ttu-id="c7a1c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c7a1c-121">Name</span></span>          | <span data-ttu-id="c7a1c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7a1c-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c7a1c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7a1c-123">Authorization</span></span> | <span data-ttu-id="c7a1c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7a1c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7a1c-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="c7a1c-126">Content-type</span></span> | <span data-ttu-id="c7a1c-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7a1c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7a1c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7a1c-129">Request body</span></span>

<span data-ttu-id="c7a1c-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7a1c-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c7a1c-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c7a1c-131">Parameter</span></span>    | <span data-ttu-id="c7a1c-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7a1c-132">Type</span></span>        | <span data-ttu-id="c7a1c-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7a1c-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c7a1c-134">mensagem</span><span class="sxs-lookup"><span data-stu-id="c7a1c-134">message</span></span>|<span data-ttu-id="c7a1c-135">String</span><span class="sxs-lookup"><span data-stu-id="c7a1c-135">String</span></span>|<span data-ttu-id="c7a1c-136">Mensagem personalizada enviada ao recusar.</span><span class="sxs-lookup"><span data-stu-id="c7a1c-136">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="c7a1c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7a1c-137">Response</span></span>

<span data-ttu-id="c7a1c-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7a1c-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7a1c-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c7a1c-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7a1c-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7a1c-141">Request</span></span>

<span data-ttu-id="c7a1c-142">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7a1c-142">The following example shows a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "offershiftrequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
Content-type: application/json

{
  "message": "Sorry, you can't offer this shift."
}
```

---


### <a name="response"></a><span data-ttu-id="c7a1c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7a1c-143">Response</span></span>

<span data-ttu-id="c7a1c-144">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="c7a1c-144">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

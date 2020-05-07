---
title: 'offerShiftRequest: aprovar'
description: Aprovar um objeto offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 98ec1f11b4364b26d478d8830a0e563ad1b7ab6b
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154946"
---
# <a name="offershiftrequest-approve"></a><span data-ttu-id="765dc-103">offerShiftRequest: aprovar</span><span class="sxs-lookup"><span data-stu-id="765dc-103">offerShiftRequest: approve</span></span>

<span data-ttu-id="765dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="765dc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="765dc-105">Aprovar um objeto [offerShiftRequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="765dc-105">Approve an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="765dc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="765dc-106">Permissions</span></span>

<span data-ttu-id="765dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="765dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="765dc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="765dc-109">Permission type</span></span>                        | <span data-ttu-id="765dc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="765dc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="765dc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="765dc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="765dc-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="765dc-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="765dc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="765dc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="765dc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="765dc-114">Not supported.</span></span> |
| <span data-ttu-id="765dc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="765dc-115">Application</span></span>                            | <span data-ttu-id="765dc-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="765dc-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="765dc-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="765dc-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="765dc-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="765dc-118">Global admins can access groups that they are not a member of.</span></span>


## <a name="http-request"></a><span data-ttu-id="765dc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="765dc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="765dc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="765dc-120">Request headers</span></span>

| <span data-ttu-id="765dc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="765dc-121">Name</span></span>          | <span data-ttu-id="765dc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="765dc-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="765dc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="765dc-123">Authorization</span></span> | <span data-ttu-id="765dc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="765dc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="765dc-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="765dc-126">Content-type</span></span> | <span data-ttu-id="765dc-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="765dc-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="765dc-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="765dc-129">Request body</span></span>

<span data-ttu-id="765dc-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="765dc-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="765dc-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="765dc-131">Parameter</span></span>    | <span data-ttu-id="765dc-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="765dc-132">Type</span></span>        | <span data-ttu-id="765dc-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="765dc-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="765dc-134">mensagem</span><span class="sxs-lookup"><span data-stu-id="765dc-134">message</span></span>|<span data-ttu-id="765dc-135">String</span><span class="sxs-lookup"><span data-stu-id="765dc-135">String</span></span>|<span data-ttu-id="765dc-136">Mensagem personalizada enviada na aprovação.</span><span class="sxs-lookup"><span data-stu-id="765dc-136">Custom message sent on approval.</span></span>|

## <a name="response"></a><span data-ttu-id="765dc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="765dc-137">Response</span></span>

<span data-ttu-id="765dc-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="765dc-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="765dc-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="765dc-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="765dc-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="765dc-141">Request</span></span>

<span data-ttu-id="765dc-142">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="765dc-142">The following example shows a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "offershiftrequest_approve"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve
Content-type: application/json

{
  "message": "Approved!"
}
```
---


### <a name="response"></a><span data-ttu-id="765dc-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="765dc-143">Response</span></span>

<span data-ttu-id="765dc-144">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="765dc-144">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: 'openShiftChangeRequest: decline'
description: Recusar uma solicitação openshift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 766faedd7fb46fb3cd6cf8434c2987e26a0ba96b
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292438"
---
# <a name="openshiftchangerequest-decline"></a><span data-ttu-id="1b772-103">openShiftChangeRequest: decline</span><span class="sxs-lookup"><span data-stu-id="1b772-103">openShiftChangeRequest: decline</span></span>

<span data-ttu-id="1b772-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b772-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b772-105">Recusar um [objeto openshiftchangerequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="1b772-105">Decline an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b772-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b772-106">Permissions</span></span>

<span data-ttu-id="1b772-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b772-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1b772-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b772-109">Permission type</span></span>                        | <span data-ttu-id="1b772-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b772-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1b772-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b772-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1b772-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b772-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1b772-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b772-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b772-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b772-114">Not supported.</span></span> |
| <span data-ttu-id="1b772-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b772-115">Application</span></span>                            | <span data-ttu-id="1b772-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b772-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b772-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b772-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="1b772-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b772-118">Request headers</span></span>

| <span data-ttu-id="1b772-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1b772-119">Name</span></span>          | <span data-ttu-id="1b772-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b772-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1b772-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b772-121">Authorization</span></span> | <span data-ttu-id="1b772-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b772-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b772-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b772-124">Request body</span></span>

<span data-ttu-id="1b772-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b772-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1b772-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1b772-126">Parameter</span></span>    | <span data-ttu-id="1b772-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b772-127">Type</span></span>        | <span data-ttu-id="1b772-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b772-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1b772-129">mensagem</span><span class="sxs-lookup"><span data-stu-id="1b772-129">message</span></span>|<span data-ttu-id="1b772-130">String</span><span class="sxs-lookup"><span data-stu-id="1b772-130">String</span></span>|<span data-ttu-id="1b772-131">Uma mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="1b772-131">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="1b772-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b772-132">Response</span></span>

<span data-ttu-id="1b772-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b772-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b772-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1b772-135">Examples</span></span>

<span data-ttu-id="1b772-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="1b772-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1b772-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b772-137">Request</span></span>

<span data-ttu-id="1b772-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b772-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="1b772-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b772-139">Response</span></span>

<span data-ttu-id="1b772-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1b772-140">The following is an example of the response.</span></span>
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
  "description": "openShiftChangeRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



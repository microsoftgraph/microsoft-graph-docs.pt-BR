---
title: 'timeOffRequest: recusar'
description: Recusar um objeto timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c0c73a983094ffae12980eeda9a12681ec9e90cb
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895521"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="4d0c7-103">timeOffRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="4d0c7-103">timeOffRequest: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d0c7-104">Recusar um objeto [timeoffrequest](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="4d0c7-104">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d0c7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d0c7-105">Permissions</span></span>

<span data-ttu-id="4d0c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d0c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d0c7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d0c7-108">Permission type</span></span>                        | <span data-ttu-id="4d0c7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d0c7-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4d0c7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d0c7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d0c7-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d0c7-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="4d0c7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d0c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d0c7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d0c7-113">Not supported.</span></span> |
| <span data-ttu-id="4d0c7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d0c7-114">Application</span></span>                            | <span data-ttu-id="4d0c7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d0c7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d0c7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d0c7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/timeOffRequests/decline
```

## <a name="request-headers"></a><span data-ttu-id="4d0c7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d0c7-117">Request headers</span></span>

| <span data-ttu-id="4d0c7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4d0c7-118">Name</span></span>          | <span data-ttu-id="4d0c7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d0c7-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4d0c7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d0c7-120">Authorization</span></span> | <span data-ttu-id="4d0c7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d0c7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d0c7-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="4d0c7-123">Content-type</span></span> | <span data-ttu-id="4d0c7-124">Application-JSON.</span><span class="sxs-lookup"><span data-stu-id="4d0c7-124">application-json.</span></span> <span data-ttu-id="4d0c7-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d0c7-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d0c7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d0c7-126">Request body</span></span>

<span data-ttu-id="4d0c7-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d0c7-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4d0c7-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4d0c7-128">Parameter</span></span>    | <span data-ttu-id="4d0c7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d0c7-129">Type</span></span>        | <span data-ttu-id="4d0c7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d0c7-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4d0c7-131">mensagem</span><span class="sxs-lookup"><span data-stu-id="4d0c7-131">message</span></span>|<span data-ttu-id="4d0c7-132">String</span><span class="sxs-lookup"><span data-stu-id="4d0c7-132">String</span></span>|<span data-ttu-id="4d0c7-133">Mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="4d0c7-133">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="4d0c7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d0c7-134">Response</span></span>

<span data-ttu-id="4d0c7-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d0c7-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4d0c7-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4d0c7-137">Examples</span></span>

<span data-ttu-id="4d0c7-138">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="4d0c7-138">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4d0c7-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d0c7-139">Request</span></span>

<span data-ttu-id="4d0c7-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d0c7-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests/decline
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="4d0c7-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d0c7-141">Response</span></span>

<span data-ttu-id="4d0c7-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4d0c7-142">The following is an example of the response.</span></span>
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
  "description": "timeOffRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

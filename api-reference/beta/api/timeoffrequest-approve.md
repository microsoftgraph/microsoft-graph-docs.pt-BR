---
title: 'timeOffRequest: aprovar'
description: Aprovar um timeoffrequest. "
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 631461eba5bab8f15bc392d59e9800f1b65be5a3
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895525"
---
# <a name="timeoffrequest-approve"></a><span data-ttu-id="5f8f9-103">timeOffRequest: aprovar</span><span class="sxs-lookup"><span data-stu-id="5f8f9-103">timeOffRequest: approve</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f8f9-104">Aprovar um [timeoffrequest](../resources/timeoffrequest.md).</span><span class="sxs-lookup"><span data-stu-id="5f8f9-104">Approve a [timeoffrequest](../resources/timeoffrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5f8f9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f8f9-105">Permissions</span></span>

<span data-ttu-id="5f8f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f8f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5f8f9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f8f9-108">Permission type</span></span>                        | <span data-ttu-id="5f8f9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f8f9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5f8f9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f8f9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f8f9-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f8f9-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="5f8f9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f8f9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f8f9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f8f9-113">Not supported.</span></span> |
| <span data-ttu-id="5f8f9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f8f9-114">Application</span></span>                            | <span data-ttu-id="5f8f9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f8f9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f8f9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f8f9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/timeOffRequests/approve
```

## <a name="request-headers"></a><span data-ttu-id="5f8f9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f8f9-117">Request headers</span></span>

| <span data-ttu-id="5f8f9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5f8f9-118">Name</span></span>          | <span data-ttu-id="5f8f9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f8f9-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5f8f9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f8f9-120">Authorization</span></span> | <span data-ttu-id="5f8f9-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="5f8f9-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f8f9-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f8f9-122">Request body</span></span>

<span data-ttu-id="5f8f9-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f8f9-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5f8f9-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5f8f9-124">Parameter</span></span>    | <span data-ttu-id="5f8f9-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f8f9-125">Type</span></span>        | <span data-ttu-id="5f8f9-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f8f9-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5f8f9-127">mensagem</span><span class="sxs-lookup"><span data-stu-id="5f8f9-127">message</span></span>|<span data-ttu-id="5f8f9-128">String</span><span class="sxs-lookup"><span data-stu-id="5f8f9-128">String</span></span>|<span data-ttu-id="5f8f9-129">Uma mensagem de aprovação personalizada.</span><span class="sxs-lookup"><span data-stu-id="5f8f9-129">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="5f8f9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f8f9-130">Response</span></span>

<span data-ttu-id="5f8f9-p102">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f8f9-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f8f9-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5f8f9-133">Examples</span></span>

<span data-ttu-id="5f8f9-134">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5f8f9-134">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="5f8f9-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f8f9-135">Request</span></span>

<span data-ttu-id="5f8f9-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f8f9-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests/approve
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="5f8f9-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f8f9-137">Response</span></span>

<span data-ttu-id="5f8f9-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5f8f9-138">The following is an example of the response.</span></span>
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
  "description": "timeOffRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

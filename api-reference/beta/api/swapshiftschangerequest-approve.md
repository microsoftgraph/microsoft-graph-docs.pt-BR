---
title: 'swapShiftsChangeRequest: aprovar'
description: Aprovar uma solicitação Shift de troca.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f952444e374d7db808dc708bf75dd9e6617d2e19
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952199"
---
# <a name="swapshiftschangerequest-approve"></a><span data-ttu-id="d86c9-103">swapShiftsChangeRequest: aprovar</span><span class="sxs-lookup"><span data-stu-id="d86c9-103">swapShiftsChangeRequest: approve</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d86c9-104">Aprovar um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="d86c9-104">Approve a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d86c9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d86c9-105">Permissions</span></span>

<span data-ttu-id="d86c9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d86c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d86c9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d86c9-108">Permission type</span></span>                        | <span data-ttu-id="d86c9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d86c9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d86c9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d86c9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d86c9-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d86c9-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d86c9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d86c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d86c9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d86c9-113">Not supported.</span></span> |
| <span data-ttu-id="d86c9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d86c9-114">Application</span></span>                            | <span data-ttu-id="d86c9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d86c9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d86c9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d86c9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/swapShiftsChangeRequests/approve
```

## <a name="request-headers"></a><span data-ttu-id="d86c9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d86c9-117">Request headers</span></span>

| <span data-ttu-id="d86c9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d86c9-118">Name</span></span>          | <span data-ttu-id="d86c9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d86c9-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d86c9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d86c9-120">Authorization</span></span> | <span data-ttu-id="d86c9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d86c9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d86c9-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="d86c9-123">Content-type</span></span> | <span data-ttu-id="d86c9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d86c9-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d86c9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d86c9-126">Request body</span></span>

<span data-ttu-id="d86c9-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d86c9-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d86c9-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d86c9-128">Parameter</span></span>    | <span data-ttu-id="d86c9-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d86c9-129">Type</span></span>        | <span data-ttu-id="d86c9-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d86c9-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d86c9-131">mensagem</span><span class="sxs-lookup"><span data-stu-id="d86c9-131">message</span></span>|<span data-ttu-id="d86c9-132">String</span><span class="sxs-lookup"><span data-stu-id="d86c9-132">String</span></span>|<span data-ttu-id="d86c9-133">Uma mensagem de aprovação personalizada.</span><span class="sxs-lookup"><span data-stu-id="d86c9-133">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="d86c9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d86c9-134">Response</span></span>

<span data-ttu-id="d86c9-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d86c9-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d86c9-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d86c9-137">Examples</span></span>

<span data-ttu-id="d86c9-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d86c9-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d86c9-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d86c9-139">Request</span></span>

<span data-ttu-id="d86c9-140">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="d86c9-140">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests/approve
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="d86c9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d86c9-141">Response</span></span>

<span data-ttu-id="d86c9-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d86c9-142">The following is an example of the response.</span></span>
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
  "description": "openShiftChangeRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

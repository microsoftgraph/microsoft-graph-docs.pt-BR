---
title: 'openShiftChangeRequest: aprovar'
description: Aprovar uma solicitação de openshift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 37af35af00f6c5f0253580f5d5034cfbd8e1f3bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019899"
---
# <a name="openshiftchangerequest-approve"></a><span data-ttu-id="e5971-103">openShiftChangeRequest: aprovar</span><span class="sxs-lookup"><span data-stu-id="e5971-103">openShiftChangeRequest: approve</span></span>

<span data-ttu-id="e5971-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5971-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5971-105">Aprovar um objeto [openshiftchangerequest](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="e5971-105">Approve an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5971-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5971-106">Permissions</span></span>

<span data-ttu-id="e5971-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5971-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5971-109">Permission type</span></span>                        | <span data-ttu-id="e5971-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5971-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e5971-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5971-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5971-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5971-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="e5971-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5971-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5971-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5971-114">Not supported.</span></span> |
| <span data-ttu-id="e5971-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5971-115">Application</span></span>                            | <span data-ttu-id="e5971-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5971-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5971-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5971-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="e5971-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5971-118">Request headers</span></span>

| <span data-ttu-id="e5971-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e5971-119">Name</span></span>          | <span data-ttu-id="e5971-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5971-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e5971-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5971-121">Authorization</span></span> | <span data-ttu-id="e5971-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5971-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5971-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="e5971-124">Content-type</span></span> | <span data-ttu-id="e5971-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5971-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5971-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5971-127">Request body</span></span>

<span data-ttu-id="e5971-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5971-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e5971-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e5971-129">Parameter</span></span>    | <span data-ttu-id="e5971-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5971-130">Type</span></span>        | <span data-ttu-id="e5971-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5971-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e5971-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="e5971-132">message</span></span>|<span data-ttu-id="e5971-133">String</span><span class="sxs-lookup"><span data-stu-id="e5971-133">String</span></span>|<span data-ttu-id="e5971-134">Uma mensagem de aprovação personalizada.</span><span class="sxs-lookup"><span data-stu-id="e5971-134">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="e5971-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5971-135">Response</span></span>

<span data-ttu-id="e5971-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5971-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e5971-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e5971-138">Examples</span></span>

<span data-ttu-id="e5971-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e5971-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="e5971-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5971-140">Request</span></span>

<span data-ttu-id="e5971-141">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5971-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="e5971-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5971-142">Response</span></span>

<span data-ttu-id="e5971-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5971-143">The following is an example of the response.</span></span>
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



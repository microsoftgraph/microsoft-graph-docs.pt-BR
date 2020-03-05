---
title: 'openShiftChangeRequest: recusar'
description: Recusar uma solicitação de openshift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 902b552a8fc6e178c3cef120ace4ea66d954812f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456382"
---
# <a name="openshiftchangerequest-decline"></a><span data-ttu-id="c36f7-103">openShiftChangeRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="c36f7-103">openShiftChangeRequest: decline</span></span>

<span data-ttu-id="c36f7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c36f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c36f7-105">Recusar um objeto [openshiftchangerequest](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="c36f7-105">Decline an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c36f7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c36f7-106">Permissions</span></span>

<span data-ttu-id="c36f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c36f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c36f7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c36f7-109">Permission type</span></span>                        | <span data-ttu-id="c36f7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c36f7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c36f7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c36f7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c36f7-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c36f7-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c36f7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c36f7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c36f7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c36f7-114">Not supported.</span></span> |
| <span data-ttu-id="c36f7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c36f7-115">Application</span></span>                            | <span data-ttu-id="c36f7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c36f7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c36f7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c36f7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="c36f7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c36f7-118">Request headers</span></span>

| <span data-ttu-id="c36f7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c36f7-119">Name</span></span>          | <span data-ttu-id="c36f7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c36f7-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c36f7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c36f7-121">Authorization</span></span> | <span data-ttu-id="c36f7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c36f7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c36f7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c36f7-124">Request body</span></span>

<span data-ttu-id="c36f7-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c36f7-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c36f7-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c36f7-126">Parameter</span></span>    | <span data-ttu-id="c36f7-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="c36f7-127">Type</span></span>        | <span data-ttu-id="c36f7-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="c36f7-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c36f7-129">mensagem</span><span class="sxs-lookup"><span data-stu-id="c36f7-129">message</span></span>|<span data-ttu-id="c36f7-130">String</span><span class="sxs-lookup"><span data-stu-id="c36f7-130">String</span></span>|<span data-ttu-id="c36f7-131">Uma mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="c36f7-131">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="c36f7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c36f7-132">Response</span></span>

<span data-ttu-id="c36f7-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c36f7-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c36f7-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c36f7-135">Examples</span></span>

<span data-ttu-id="c36f7-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="c36f7-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c36f7-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c36f7-137">Request</span></span>

<span data-ttu-id="c36f7-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c36f7-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="c36f7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c36f7-139">Response</span></span>

<span data-ttu-id="c36f7-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c36f7-140">The following is an example of the response.</span></span>
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

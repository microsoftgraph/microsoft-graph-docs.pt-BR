---
title: 'offerShiftRequest: recusar'
description: Recusar uma solicitação de mudança de oferta.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6d6b6ec17b574e23c08beee85d77e5a61e2f4c5a
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44153986"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="a761a-103">offerShiftRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="a761a-103">offerShiftRequest: decline</span></span>

<span data-ttu-id="a761a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a761a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a761a-105">Recusar um objeto [offershiftrequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="a761a-105">Decline an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a761a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a761a-106">Permissions</span></span>

<span data-ttu-id="a761a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a761a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a761a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a761a-109">Permission type</span></span>                        | <span data-ttu-id="a761a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a761a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a761a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a761a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a761a-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a761a-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="a761a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a761a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a761a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a761a-114">Not supported.</span></span> |
| <span data-ttu-id="a761a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a761a-115">Application</span></span>                            | <span data-ttu-id="a761a-116">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="a761a-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="a761a-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="a761a-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="a761a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a761a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="a761a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a761a-119">Request headers</span></span>

| <span data-ttu-id="a761a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a761a-120">Name</span></span>          | <span data-ttu-id="a761a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a761a-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a761a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a761a-122">Authorization</span></span> | <span data-ttu-id="a761a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a761a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a761a-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="a761a-125">Content-type</span></span> | <span data-ttu-id="a761a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a761a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a761a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a761a-128">Request body</span></span>

<span data-ttu-id="a761a-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a761a-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a761a-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a761a-130">Parameter</span></span>    | <span data-ttu-id="a761a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a761a-131">Type</span></span>        | <span data-ttu-id="a761a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a761a-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a761a-133">mensagem</span><span class="sxs-lookup"><span data-stu-id="a761a-133">message</span></span>|<span data-ttu-id="a761a-134">String</span><span class="sxs-lookup"><span data-stu-id="a761a-134">String</span></span>|<span data-ttu-id="a761a-135">Mensagem personalizada enviada ao recusar.</span><span class="sxs-lookup"><span data-stu-id="a761a-135">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="a761a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a761a-136">Response</span></span>

<span data-ttu-id="a761a-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a761a-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a761a-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a761a-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a761a-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a761a-140">Request</span></span>

<span data-ttu-id="a761a-141">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a761a-141">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a761a-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="a761a-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
Content-type: application/json

{
  "message": "Sorry, you can't offer this shift."
}
```
# <a name="javascript"></a>[<span data-ttu-id="a761a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a761a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a761a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a761a-144">Response</span></span>

<span data-ttu-id="a761a-145">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="a761a-145">The following example shows the response.</span></span>
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

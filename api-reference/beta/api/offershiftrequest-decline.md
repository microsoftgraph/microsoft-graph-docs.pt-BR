---
title: 'offerShiftRequest: recusar'
description: Recusar uma solicitação de mudança de oferta.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 92a085bb089c549bf4860dcbce135cd4f887ea48
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994926"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="8541d-103">offerShiftRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="8541d-103">offerShiftRequest: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8541d-104">Recusar um objeto [offershiftrequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="8541d-104">Decline an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8541d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8541d-105">Permissions</span></span>

<span data-ttu-id="8541d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8541d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8541d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8541d-108">Permission type</span></span>                        | <span data-ttu-id="8541d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8541d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8541d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8541d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8541d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8541d-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="8541d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8541d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8541d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8541d-113">Not supported.</span></span> |
| <span data-ttu-id="8541d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8541d-114">Application</span></span>                            | <span data-ttu-id="8541d-115">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="8541d-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="8541d-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="8541d-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="8541d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8541d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/schedule/offerShiftRequests/decline
```

## <a name="request-headers"></a><span data-ttu-id="8541d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8541d-118">Request headers</span></span>

| <span data-ttu-id="8541d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8541d-119">Name</span></span>          | <span data-ttu-id="8541d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8541d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8541d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8541d-121">Authorization</span></span> | <span data-ttu-id="8541d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8541d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8541d-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="8541d-124">Content-type</span></span> | <span data-ttu-id="8541d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8541d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8541d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8541d-127">Request body</span></span>

<span data-ttu-id="8541d-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8541d-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8541d-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8541d-129">Parameter</span></span>    | <span data-ttu-id="8541d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8541d-130">Type</span></span>        | <span data-ttu-id="8541d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8541d-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8541d-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="8541d-132">message</span></span>|<span data-ttu-id="8541d-133">String</span><span class="sxs-lookup"><span data-stu-id="8541d-133">String</span></span>|<span data-ttu-id="8541d-134">Mensagem personalizada enviada ao recusar.</span><span class="sxs-lookup"><span data-stu-id="8541d-134">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="8541d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8541d-135">Response</span></span>

<span data-ttu-id="8541d-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8541d-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8541d-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8541d-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8541d-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8541d-139">Request</span></span>

<span data-ttu-id="8541d-140">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="8541d-140">The following example shows a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8541d-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="8541d-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/schedule/offerShiftRequests/decline
Content-type: application/json

{
  "message": "Sorry, you can't offer this shift."
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8541d-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8541d-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8541d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="8541d-143">Response</span></span>

<span data-ttu-id="8541d-144">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="8541d-144">The following example shows the response.</span></span>
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

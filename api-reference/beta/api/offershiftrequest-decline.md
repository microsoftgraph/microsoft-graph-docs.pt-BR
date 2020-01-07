---
title: 'offerShiftRequest: recusar'
description: Recusar uma solicitação de mudança de oferta.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 960532d3d278bc01ae89bc74a8624030c96c6d96
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952171"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="500f4-103">offerShiftRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="500f4-103">offerShiftRequest: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="500f4-104">Recusar um objeto [offershiftrequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="500f4-104">Decline an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="500f4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="500f4-105">Permissions</span></span>

<span data-ttu-id="500f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="500f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="500f4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="500f4-108">Permission type</span></span>                        | <span data-ttu-id="500f4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="500f4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="500f4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="500f4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="500f4-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="500f4-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="500f4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="500f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="500f4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="500f4-113">Not supported.</span></span> |
| <span data-ttu-id="500f4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="500f4-114">Application</span></span>                            | <span data-ttu-id="500f4-115">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="500f4-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="500f4-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="500f4-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="500f4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="500f4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/schedule/offerShiftRequests/decline
```

## <a name="request-headers"></a><span data-ttu-id="500f4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="500f4-118">Request headers</span></span>

| <span data-ttu-id="500f4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="500f4-119">Name</span></span>          | <span data-ttu-id="500f4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="500f4-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="500f4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="500f4-121">Authorization</span></span> | <span data-ttu-id="500f4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="500f4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="500f4-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="500f4-124">Content-type</span></span> | <span data-ttu-id="500f4-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="500f4-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="500f4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="500f4-127">Request body</span></span>

<span data-ttu-id="500f4-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="500f4-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="500f4-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="500f4-129">Parameter</span></span>    | <span data-ttu-id="500f4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="500f4-130">Type</span></span>        | <span data-ttu-id="500f4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="500f4-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="500f4-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="500f4-132">message</span></span>|<span data-ttu-id="500f4-133">String</span><span class="sxs-lookup"><span data-stu-id="500f4-133">String</span></span>|<span data-ttu-id="500f4-134">Mensagem personalizada enviada ao recusar.</span><span class="sxs-lookup"><span data-stu-id="500f4-134">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="500f4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="500f4-135">Response</span></span>

<span data-ttu-id="500f4-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="500f4-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="500f4-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="500f4-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="500f4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="500f4-139">Request</span></span>

<span data-ttu-id="500f4-140">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="500f4-140">The following example shows a request.</span></span>
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

### <a name="response"></a><span data-ttu-id="500f4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="500f4-141">Response</span></span>

<span data-ttu-id="500f4-142">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="500f4-142">The following example shows the response.</span></span>
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

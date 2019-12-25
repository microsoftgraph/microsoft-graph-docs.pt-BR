---
title: 'timeOffRequest: recusar'
description: Recusar um objeto timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 69dce3ef9a9486e204eca58421aff606b56385aa
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863615"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="8f502-103">timeOffRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="8f502-103">timeOffRequest: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f502-104">Recusar um objeto [timeoffrequest](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="8f502-104">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f502-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f502-105">Permissions</span></span>

<span data-ttu-id="8f502-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f502-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f502-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f502-108">Permission type</span></span>                        | <span data-ttu-id="8f502-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f502-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8f502-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f502-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f502-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f502-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="8f502-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f502-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f502-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f502-113">Not supported.</span></span> |
|<span data-ttu-id="8f502-114">Application</span><span class="sxs-lookup"><span data-stu-id="8f502-114">Application</span></span> | <span data-ttu-id="8f502-115">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="8f502-115">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="8f502-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="8f502-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="8f502-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f502-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/timeOffRequests/decline
```

## <a name="request-headers"></a><span data-ttu-id="8f502-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f502-118">Request headers</span></span>

| <span data-ttu-id="8f502-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8f502-119">Name</span></span>          | <span data-ttu-id="8f502-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f502-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8f502-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f502-121">Authorization</span></span> | <span data-ttu-id="8f502-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f502-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f502-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="8f502-124">Content-type</span></span> | <span data-ttu-id="8f502-125">Application-JSON.</span><span class="sxs-lookup"><span data-stu-id="8f502-125">application-json.</span></span> <span data-ttu-id="8f502-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f502-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f502-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f502-127">Request body</span></span>

<span data-ttu-id="8f502-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f502-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8f502-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8f502-129">Parameter</span></span>    | <span data-ttu-id="8f502-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f502-130">Type</span></span>        | <span data-ttu-id="8f502-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f502-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8f502-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="8f502-132">message</span></span>|<span data-ttu-id="8f502-133">String</span><span class="sxs-lookup"><span data-stu-id="8f502-133">String</span></span>|<span data-ttu-id="8f502-134">Mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="8f502-134">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="8f502-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f502-135">Response</span></span>

<span data-ttu-id="8f502-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f502-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f502-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8f502-138">Examples</span></span>

<span data-ttu-id="8f502-139">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8f502-139">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8f502-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f502-140">Request</span></span>

<span data-ttu-id="8f502-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f502-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8f502-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f502-142">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f502-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f502-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f502-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f502-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8f502-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f502-145">Response</span></span>

<span data-ttu-id="8f502-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f502-146">The following is an example of the response.</span></span>
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

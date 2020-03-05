---
title: 'offerShiftRequest: aprovar'
description: Aprovar um objeto offershiftrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aef00c4de700624eac54e3aca8bbc2773799b377
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456604"
---
# <a name="offershiftrequest-approve"></a><span data-ttu-id="df748-103">offerShiftRequest: aprovar</span><span class="sxs-lookup"><span data-stu-id="df748-103">offerShiftRequest: approve</span></span>

<span data-ttu-id="df748-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="df748-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df748-105">Aprovar um objeto [offershiftrequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="df748-105">Approve an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="df748-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="df748-106">Permissions</span></span>

<span data-ttu-id="df748-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df748-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df748-109">Permission type</span></span>                        | <span data-ttu-id="df748-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df748-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="df748-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df748-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="df748-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df748-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="df748-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df748-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df748-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df748-114">Not supported.</span></span> |
| <span data-ttu-id="df748-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df748-115">Application</span></span>                            | <span data-ttu-id="df748-116">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="df748-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="df748-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="df748-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="df748-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df748-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/schedule/offerShiftRequests/approve
```

## <a name="request-headers"></a><span data-ttu-id="df748-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df748-119">Request headers</span></span>

| <span data-ttu-id="df748-120">Nome</span><span class="sxs-lookup"><span data-stu-id="df748-120">Name</span></span>          | <span data-ttu-id="df748-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="df748-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="df748-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="df748-122">Authorization</span></span> | <span data-ttu-id="df748-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df748-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="df748-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="df748-125">Content-type</span></span> | <span data-ttu-id="df748-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df748-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df748-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df748-128">Request body</span></span>

<span data-ttu-id="df748-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df748-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="df748-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="df748-130">Parameter</span></span>    | <span data-ttu-id="df748-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="df748-131">Type</span></span>        | <span data-ttu-id="df748-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="df748-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df748-133">mensagem</span><span class="sxs-lookup"><span data-stu-id="df748-133">message</span></span>|<span data-ttu-id="df748-134">String</span><span class="sxs-lookup"><span data-stu-id="df748-134">String</span></span>|<span data-ttu-id="df748-135">Mensagem personalizada enviada na aprovação.</span><span class="sxs-lookup"><span data-stu-id="df748-135">Custom message sent on approval.</span></span>|

## <a name="response"></a><span data-ttu-id="df748-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="df748-136">Response</span></span>

<span data-ttu-id="df748-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df748-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df748-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="df748-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="df748-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df748-140">Request</span></span>

<span data-ttu-id="df748-141">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="df748-141">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="df748-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="df748-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/schedule/offerShiftRequests/approve
Content-type: application/json

{
  "message": "Approved!"
}
```
# <a name="javascript"></a>[<span data-ttu-id="df748-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df748-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="df748-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="df748-144">Response</span></span>

<span data-ttu-id="df748-145">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="df748-145">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

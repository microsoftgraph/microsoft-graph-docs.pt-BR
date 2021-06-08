---
title: 'timeOffRequest: aprovar'
description: Aprovar um objeto timeoffrequest."
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 291a3e764ebcd84d181b5441405c4579cf798dc2
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787318"
---
# <a name="timeoffrequest-approve"></a><span data-ttu-id="a40b3-103">timeOffRequest: aprovar</span><span class="sxs-lookup"><span data-stu-id="a40b3-103">timeOffRequest: approve</span></span>

<span data-ttu-id="a40b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a40b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a40b3-105">Aprovar um [período de tempo limite](../resources/timeoffrequest.md).</span><span class="sxs-lookup"><span data-stu-id="a40b3-105">Approve a [timeoffrequest](../resources/timeoffrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a40b3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a40b3-106">Permissions</span></span>

<span data-ttu-id="a40b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a40b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a40b3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a40b3-109">Permission type</span></span>                        | <span data-ttu-id="a40b3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a40b3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a40b3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a40b3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a40b3-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a40b3-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="a40b3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a40b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a40b3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a40b3-114">Not supported.</span></span> |
|<span data-ttu-id="a40b3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a40b3-115">Application</span></span> | <span data-ttu-id="a40b3-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="a40b3-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="a40b3-117">\***Importante:** As permissões de aplicativo estão atualmente apenas em visualização privada e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="a40b3-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="a40b3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a40b3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="a40b3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a40b3-119">Request headers</span></span>

| <span data-ttu-id="a40b3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a40b3-120">Name</span></span>          | <span data-ttu-id="a40b3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a40b3-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a40b3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a40b3-122">Authorization</span></span> | <span data-ttu-id="a40b3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a40b3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a40b3-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="a40b3-125">Content-type</span></span> | <span data-ttu-id="a40b3-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a40b3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a40b3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a40b3-128">Request body</span></span>

<span data-ttu-id="a40b3-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a40b3-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a40b3-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a40b3-130">Parameter</span></span>    | <span data-ttu-id="a40b3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a40b3-131">Type</span></span>        | <span data-ttu-id="a40b3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a40b3-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a40b3-133">mensagem</span><span class="sxs-lookup"><span data-stu-id="a40b3-133">message</span></span>|<span data-ttu-id="a40b3-134">String</span><span class="sxs-lookup"><span data-stu-id="a40b3-134">String</span></span>|<span data-ttu-id="a40b3-135">Mensagem de aprovação personalizada.</span><span class="sxs-lookup"><span data-stu-id="a40b3-135">Custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="a40b3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a40b3-136">Response</span></span>

<span data-ttu-id="a40b3-p104">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a40b3-p104">If successful, this method returns a `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a40b3-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a40b3-139">Examples</span></span>

<span data-ttu-id="a40b3-140">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a40b3-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a40b3-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a40b3-141">Request</span></span>

<span data-ttu-id="a40b3-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a40b3-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a40b3-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="a40b3-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="javascript"></a>[<span data-ttu-id="a40b3-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a40b3-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a40b3-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a40b3-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="a40b3-146">C#</span><span class="sxs-lookup"><span data-stu-id="a40b3-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffrequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a40b3-147">Java</span><span class="sxs-lookup"><span data-stu-id="a40b3-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffrequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a40b3-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a40b3-148">Response</span></span>

<span data-ttu-id="a40b3-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a40b3-149">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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



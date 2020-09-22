---
title: 'timeOffRequest: aprovar'
description: Aprovar um objeto timeoffrequest. "
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dd12448bf0e20824c7b3baa67caddfbe42f0595e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023041"
---
# <a name="timeoffrequest-approve"></a><span data-ttu-id="4397a-103">timeOffRequest: aprovar</span><span class="sxs-lookup"><span data-stu-id="4397a-103">timeOffRequest: approve</span></span>

<span data-ttu-id="4397a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4397a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4397a-105">Aprovar um [timeoffrequest](../resources/timeoffrequest.md).</span><span class="sxs-lookup"><span data-stu-id="4397a-105">Approve a [timeoffrequest](../resources/timeoffrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4397a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4397a-106">Permissions</span></span>

<span data-ttu-id="4397a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4397a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4397a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4397a-109">Permission type</span></span>                        | <span data-ttu-id="4397a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4397a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="4397a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4397a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4397a-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4397a-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4397a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4397a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4397a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4397a-114">Not supported.</span></span>    |
|<span data-ttu-id="4397a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4397a-115">Application</span></span> | <span data-ttu-id="4397a-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4397a-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="4397a-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="4397a-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4397a-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="4397a-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4397a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4397a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="4397a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4397a-120">Request headers</span></span>

| <span data-ttu-id="4397a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4397a-121">Name</span></span>          | <span data-ttu-id="4397a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4397a-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4397a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4397a-123">Authorization</span></span> | <span data-ttu-id="4397a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4397a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4397a-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="4397a-126">Content-type</span></span> | <span data-ttu-id="4397a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4397a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4397a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4397a-129">Request body</span></span>

<span data-ttu-id="4397a-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4397a-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4397a-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4397a-131">Parameter</span></span>    | <span data-ttu-id="4397a-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="4397a-132">Type</span></span>        | <span data-ttu-id="4397a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="4397a-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4397a-134">mensagem</span><span class="sxs-lookup"><span data-stu-id="4397a-134">message</span></span>|<span data-ttu-id="4397a-135">String</span><span class="sxs-lookup"><span data-stu-id="4397a-135">String</span></span>|<span data-ttu-id="4397a-136">Mensagem de aprovação personalizada.</span><span class="sxs-lookup"><span data-stu-id="4397a-136">Custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="4397a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4397a-137">Response</span></span>

<span data-ttu-id="4397a-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4397a-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4397a-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4397a-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4397a-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4397a-141">Request</span></span>

<span data-ttu-id="4397a-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4397a-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4397a-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="4397a-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_approve"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="4397a-144">C#</span><span class="sxs-lookup"><span data-stu-id="4397a-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffrequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4397a-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4397a-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4397a-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4397a-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4397a-147">Java</span><span class="sxs-lookup"><span data-stu-id="4397a-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffrequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="4397a-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="4397a-148">Response</span></span>

<span data-ttu-id="4397a-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4397a-149">The following is an example of the response.</span></span>
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


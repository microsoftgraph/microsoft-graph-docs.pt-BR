---
title: Excluir timeOffRequest
description: Excluir um objeto timeOffRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 97587997d771fee433b72d54347dc05aa73acb72
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863588"
---
# <a name="delete-timeoffrequest"></a><span data-ttu-id="bd62f-103">Excluir timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="bd62f-103">Delete timeOffRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd62f-104">Excluir um objeto [timeOffRequest](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="bd62f-104">Delete a [timeOffRequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd62f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd62f-105">Permissions</span></span>

<span data-ttu-id="bd62f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd62f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd62f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd62f-108">Permission type</span></span>                        | <span data-ttu-id="bd62f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd62f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bd62f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd62f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd62f-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd62f-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="bd62f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd62f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd62f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd62f-113">Not supported.</span></span> |
|<span data-ttu-id="bd62f-114">Application</span><span class="sxs-lookup"><span data-stu-id="bd62f-114">Application</span></span> | <span data-ttu-id="bd62f-115">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="bd62f-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="bd62f-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="bd62f-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="bd62f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd62f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/timeOffRequests
```

## <a name="request-headers"></a><span data-ttu-id="bd62f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd62f-118">Request headers</span></span>

| <span data-ttu-id="bd62f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bd62f-119">Name</span></span>          | <span data-ttu-id="bd62f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd62f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bd62f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd62f-121">Authorization</span></span> | <span data-ttu-id="bd62f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd62f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd62f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd62f-124">Request body</span></span>

<span data-ttu-id="bd62f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd62f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd62f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd62f-126">Response</span></span>

<span data-ttu-id="bd62f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd62f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd62f-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bd62f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd62f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd62f-130">Request</span></span>

<span data-ttu-id="bd62f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd62f-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bd62f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd62f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_timeoffrequest"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bd62f-133">C#</span><span class="sxs-lookup"><span data-stu-id="bd62f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd62f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd62f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bd62f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd62f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd62f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd62f-136">Response</span></span>

<span data-ttu-id="bd62f-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bd62f-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

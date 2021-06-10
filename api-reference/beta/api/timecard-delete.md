---
title: Excluir timeCard
description: Exclua uma instância timeCard na agenda.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fc76b48ac1bac83435446d50e93a93ef256a49be
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869727"
---
# <a name="delete-timecard"></a><span data-ttu-id="5b031-103">Excluir timeCard</span><span class="sxs-lookup"><span data-stu-id="5b031-103">Delete timeCard</span></span>

<span data-ttu-id="5b031-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b031-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b031-105">[Exclua uma instância de cartão](../resources/timeCard.md) de tempo em um [agendamento](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="5b031-105">Delete a [timeCard](../resources/timeCard.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b031-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="5b031-106">Permissions</span></span>

<span data-ttu-id="5b031-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b031-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b031-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b031-109">Permission type</span></span>      | <span data-ttu-id="5b031-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b031-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b031-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b031-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5b031-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b031-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="5b031-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b031-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b031-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b031-114">Not supported.</span></span>    |
|<span data-ttu-id="5b031-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b031-115">Application</span></span> | <span data-ttu-id="5b031-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="5b031-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="5b031-117">\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b031-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="5b031-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b031-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timecards/{timeCardID}
```

## <a name="request-headers"></a><span data-ttu-id="5b031-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b031-119">Request headers</span></span>

| <span data-ttu-id="5b031-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b031-120">Header</span></span>       | <span data-ttu-id="5b031-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5b031-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5b031-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b031-122">Authorization</span></span>  | <span data-ttu-id="5b031-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b031-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5b031-125">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="5b031-125">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="5b031-126">A ID do usuário em nome do qual o aplicativo está agindo.</span><span class="sxs-lookup"><span data-stu-id="5b031-126">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="5b031-127">Obrigatório ao usar o escopo de permissão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5b031-127">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b031-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b031-128">Request body</span></span>
<span data-ttu-id="5b031-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b031-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b031-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b031-130">Response</span></span>

<span data-ttu-id="5b031-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5b031-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5b031-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b031-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b031-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b031-133">Request</span></span>
<span data-ttu-id="5b031-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b031-134">The following is an example of the request.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5b031-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b031-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-delete"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule/timecards/3895809b-a618-4c0d-86a0-d42b25b7d74f
```
# <a name="c"></a>[<span data-ttu-id="5b031-136">C#</span><span class="sxs-lookup"><span data-stu-id="5b031-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timecard-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b031-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b031-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b031-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b031-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5b031-139">Java</span><span class="sxs-lookup"><span data-stu-id="5b031-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timecard-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5b031-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b031-140">Response</span></span>

<span data-ttu-id="5b031-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5b031-141">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete timeCard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

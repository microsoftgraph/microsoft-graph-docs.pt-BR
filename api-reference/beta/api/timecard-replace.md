---
title: Substituir timeCard
description: Atualize uma entrada de cartão de ponto existente.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cbfb5f30991ebd8ae2c2208a1e366557c6eafc1c
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870448"
---
# <a name="replace-timecard"></a><span data-ttu-id="a7564-103">Substituir timeCard</span><span class="sxs-lookup"><span data-stu-id="a7564-103">Replace timeCard</span></span>

<span data-ttu-id="a7564-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7564-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7564-105">Substitua um [cartão](../resources/timecard.md) de ponto existente por valores atualizados.</span><span class="sxs-lookup"><span data-stu-id="a7564-105">Replace an existing [timeCard](../resources/timecard.md) with updated values.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7564-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a7564-106">Permissions</span></span>

<span data-ttu-id="a7564-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7564-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7564-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7564-109">Permission type</span></span>      | <span data-ttu-id="a7564-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7564-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7564-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7564-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a7564-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7564-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="a7564-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7564-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7564-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7564-114">Not supported.</span></span>    |
|<span data-ttu-id="a7564-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7564-115">Application</span></span> | <span data-ttu-id="a7564-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="a7564-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="a7564-117">\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7564-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="a7564-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7564-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timecards/{timeCardID}
```

## <a name="request-headers"></a><span data-ttu-id="a7564-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7564-119">Request headers</span></span>

| <span data-ttu-id="a7564-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7564-120">Header</span></span>       | <span data-ttu-id="a7564-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a7564-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a7564-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7564-122">Authorization</span></span>  | <span data-ttu-id="a7564-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7564-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a7564-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a7564-125">Content-Type</span></span>  | <span data-ttu-id="a7564-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7564-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="a7564-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="a7564-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="a7564-129">A ID do usuário em nome do qual o aplicativo está agindo.</span><span class="sxs-lookup"><span data-stu-id="a7564-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="a7564-130">Obrigatório ao usar o escopo de permissão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a7564-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7564-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7564-131">Request body</span></span>

<span data-ttu-id="a7564-132">No corpo da solicitação, fornece uma representação JSON de um [objeto timeCard.](../resources/timecard.md)</span><span class="sxs-lookup"><span data-stu-id="a7564-132">In the request body, supply a JSON representation of a [timeCard](../resources/timecard.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a7564-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7564-133">Response</span></span>

<span data-ttu-id="a7564-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a7564-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a7564-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a7564-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a7564-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7564-136">Request</span></span>

<span data-ttu-id="a7564-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7564-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a7564-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7564-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard_replace"
}-->

```http
PUT https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_3cd7413f-0337-433b-9a49-da0923185b3f
Content-type: application/json

{
    "userId": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
    "state": "clockedOut",
    "confirmedBy": "None",
    "notes": null,
    "clockInEvent": {
        "dateTime": "2021-05-21T21:58:41.327Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "update sample notes"
        }
    },
    "clockOutEvent": {
        "dateTime": "2021-05-21T22:01:46.205Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "update sample notes"
        }
    },
    "breaks": [
        {
            "breakId": "BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f",
            "notes": null,
            "start": {
                "dateTime": "2021-05-21T21:59:59.328Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "update sample notes"
                }
            },
            "end": {
                "dateTime": "2021-05-21T22:01:10.205Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "update sample notes"
                }
            }
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="a7564-139">C#</span><span class="sxs-lookup"><span data-stu-id="a7564-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timecard-replace-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7564-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7564-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-replace-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7564-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7564-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-replace-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a7564-142">Java</span><span class="sxs-lookup"><span data-stu-id="a7564-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timecard-replace-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a7564-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7564-143">Response</span></span>

<span data-ttu-id="a7564-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a7564-144">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "timecard_replace"
} -->

```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing timeCard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

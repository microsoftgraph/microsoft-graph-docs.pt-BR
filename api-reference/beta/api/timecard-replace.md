---
title: Substituir timeCard
description: Atualize uma entrada de cartão de ponto existente.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 095c5fcdda15496ab41570aa940ad09585f9a633
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787833"
---
# <a name="replace-timecard"></a><span data-ttu-id="7d033-103">Substituir timeCard</span><span class="sxs-lookup"><span data-stu-id="7d033-103">Replace timeCard</span></span>

<span data-ttu-id="7d033-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d033-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d033-105">Substitua um [cartão](../resources/timecard.md) de ponto existente por valores atualizados.</span><span class="sxs-lookup"><span data-stu-id="7d033-105">Replace an existing [timeCard](../resources/timecard.md) with updated values.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d033-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7d033-106">Permissions</span></span>

<span data-ttu-id="7d033-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d033-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d033-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d033-109">Permission type</span></span>      | <span data-ttu-id="7d033-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d033-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d033-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d033-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7d033-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d033-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="7d033-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d033-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d033-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d033-114">Not supported.</span></span>    |
|<span data-ttu-id="7d033-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d033-115">Application</span></span> | <span data-ttu-id="7d033-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="7d033-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="7d033-117">\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d033-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="7d033-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d033-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timecards/{timeCardID}
```

## <a name="request-headers"></a><span data-ttu-id="7d033-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d033-119">Request headers</span></span>

| <span data-ttu-id="7d033-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d033-120">Header</span></span>       | <span data-ttu-id="7d033-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7d033-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7d033-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d033-122">Authorization</span></span>  | <span data-ttu-id="7d033-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d033-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7d033-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7d033-125">Content-Type</span></span>  | <span data-ttu-id="7d033-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d033-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="7d033-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="7d033-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="7d033-129">A ID do usuário em nome do qual o aplicativo está agindo.</span><span class="sxs-lookup"><span data-stu-id="7d033-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="7d033-130">Obrigatório ao usar o escopo de permissão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7d033-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d033-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d033-131">Request body</span></span>

<span data-ttu-id="7d033-132">No corpo da solicitação, fornece uma representação JSON de um [objeto timeCard.](../resources/timecard.md)</span><span class="sxs-lookup"><span data-stu-id="7d033-132">In the request body, supply a JSON representation of a [timeCard](../resources/timecard.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7d033-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d033-133">Response</span></span>

<span data-ttu-id="7d033-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7d033-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7d033-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7d033-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7d033-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d033-136">Request</span></span>

<span data-ttu-id="7d033-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d033-137">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d033-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d033-138">Response</span></span>

<span data-ttu-id="7d033-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7d033-139">The following is an example of the response.</span></span> 
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

---
title: Criar timeCard
description: Crie uma instância timeCard na agenda.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e1a03dd2139070fa06156689bf332d0e7c1a3dcb
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870091"
---
# <a name="create-timecard"></a><span data-ttu-id="fe6ad-103">Criar timeCard</span><span class="sxs-lookup"><span data-stu-id="fe6ad-103">Create timeCard</span></span>

<span data-ttu-id="fe6ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe6ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe6ad-105">Crie uma [instância do timeCard](../resources/timeCard.md) em um [agendamento](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="fe6ad-105">Create a [timeCard](../resources/timeCard.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fe6ad-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="fe6ad-106">Permissions</span></span>

<span data-ttu-id="fe6ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe6ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe6ad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe6ad-109">Permission type</span></span>      | <span data-ttu-id="fe6ad-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe6ad-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe6ad-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe6ad-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fe6ad-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe6ad-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe6ad-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe6ad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe6ad-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe6ad-114">Not supported.</span></span>    |
|<span data-ttu-id="fe6ad-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe6ad-115">Application</span></span> | <span data-ttu-id="fe6ad-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="fe6ad-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="fe6ad-117">\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe6ad-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="fe6ad-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe6ad-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards
```

## <a name="request-headers"></a><span data-ttu-id="fe6ad-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe6ad-119">Request headers</span></span>

| <span data-ttu-id="fe6ad-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe6ad-120">Header</span></span>       | <span data-ttu-id="fe6ad-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fe6ad-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fe6ad-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe6ad-122">Authorization</span></span>  | <span data-ttu-id="fe6ad-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe6ad-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fe6ad-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="fe6ad-125">Content-type</span></span> | <span data-ttu-id="fe6ad-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe6ad-p103">application/json. Required.</span></span>|
| <span data-ttu-id="fe6ad-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="fe6ad-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="fe6ad-129">A ID do usuário em nome do qual o aplicativo está agindo.</span><span class="sxs-lookup"><span data-stu-id="fe6ad-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="fe6ad-130">Obrigatório ao usar o escopo de permissão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fe6ad-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe6ad-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe6ad-131">Request body</span></span>

<span data-ttu-id="fe6ad-132">Forneça o novo [objeto timeCard](../resources/timecard.md) no corpo da solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="fe6ad-132">Provide the new [timeCard](../resources/timecard.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe6ad-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe6ad-133">Response</span></span>

<span data-ttu-id="fe6ad-134">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [timeCard](../resources/timeCard.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe6ad-134">If successful, this method returns a `201 Created` response code and a [timeCard](../resources/timeCard.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe6ad-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe6ad-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe6ad-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe6ad-136">Request</span></span>
<span data-ttu-id="fe6ad-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe6ad-137">The following is an example of the request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="fe6ad-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe6ad-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-post"
}-->

```http
POST https://graph.microsoft.com/beta/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule/timecards
Content-type: application/json

{
  "onBehalfOfUserId":"a3601044-a1b5-438e-b742-f78d01d68a67",
  "clockInEvent":{
     "dateTime":"2019-03-18T00:00:00.000Z",
     "atApprovedLocation":true,
     "notes": {
        "content": "Started late due to traffic in CA 237",
        "contentType": "text"
     },
  },
  "notes":{
        "content": "8 To 5 Inventory management",
        "contentType": "text"
   },
  "breaks":[
     {
       "breakId": "string",
        "notes":{
             "content": "Lunch break",
             "contentType": "text"
        },
        "start":{
           "dateTime":"2019-03-18T02:00:00.000Z",
           "atApprovedLocation":true,
           "notes": {
                "content": "Reduced break to make up for lost time",
                "contentType": "text"
             },
        }
     }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="fe6ad-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe6ad-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe6ad-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe6ad-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fe6ad-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe6ad-141">Response</span></span>

<span data-ttu-id="fe6ad-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fe6ad-142">The following is an example of the response.</span></span> 

><span data-ttu-id="fe6ad-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fe6ad-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "id":"3895809b-a618-4c0d-86a0-d42b25b7d74f",
   "userId":"a3601044-a1b5-438e-b742-f78d01d68a67",
   "createdDateTime":"2019-03-18T00:00:00.000Z",
   "createdBy":{
      "user":{
         "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
         "displayName":"Dwight Schrute"
      }
   },
   "lastModifiedDateTime":"2019-03-18T00:00:00.000Z",
   "lastModifiedBy":{
      "user":{
         "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
         "displayName":"Dwight Schrute"
      }
   },
   "state":"onBreak",
   "confirmationStatus":"notConfirmed",
   "originalEntry":{
      "clockInEvent":{
         "dateTime":"2019-03-18T00:00:00.000Z",
         "atApprovedLocation":true,
         "notes": {
            "content": "Started late due to traffic in CA 237",
           "contentType": "text"
         },
      },
      "clockOutEvent":null,
      "breaks":[
         {
            "breakId":"string",
            "notes":{
                "content": "Lunch break",
                "contentType": "text"
             },
            "start":{
               "dateTime":"2019-03-18T02:00:00.000Z",
               "atApprovedLocation":true,
               "notes": {
                  "content": "Reduced break to make up for lost time",
                  "contentType": "text"
               },
            },
            "end":null
         }
      ]
   },
   "clockInEvent":{
      "dateTime":"2019-03-18T00:00:00.000Z",
      "atApprovedLocation":true,
      "notes": {
        "content": "Started late due to traffic in CA 237",
        "contentType": "text"
     },
   },
   "clockOutEvent":null,
   "notes":{
        "content": "8 To 5 Inventory management",
        "contentType": "text"
   },
   "breaks":[
      {
         "breakId":"string",
         "notes":{
             "content": "Lunch break",
             "contentType": "text"
         },
         "start":{
            "dateTime":"2019-03-18T02:00:00.000Z",
            "atApprovedLocation":true,
            "notes": {
                "content": "Reduced break to make up for lost time",
                "contentType": "text"
             },
         },
         "end":null
      }
   ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create timeCard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

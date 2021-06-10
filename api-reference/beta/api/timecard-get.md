---
title: Obter timeCard
description: Obter um cartão de ponto por ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3ffeb7f57769cc84500b9c0dbb913c214ba6e144
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869511"
---
# <a name="get-timecard"></a><span data-ttu-id="4f06d-103">Obter timeCard</span><span class="sxs-lookup"><span data-stu-id="4f06d-103">Get timeCard</span></span>

<span data-ttu-id="4f06d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f06d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f06d-105">Recupere as propriedades e as relações de um [objeto timeCard](../resources/timeCard.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="4f06d-105">Retrieve the properties and relationships of a [timeCard](../resources/timeCard.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f06d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4f06d-106">Permissions</span></span>

<span data-ttu-id="4f06d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f06d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f06d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f06d-109">Permission type</span></span>      | <span data-ttu-id="4f06d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f06d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f06d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f06d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4f06d-112">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f06d-112">Schedule.Read.All, Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="4f06d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f06d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f06d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f06d-114">Not supported.</span></span>    |
|<span data-ttu-id="4f06d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f06d-115">Application</span></span> | <span data-ttu-id="4f06d-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="4f06d-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="4f06d-117">\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f06d-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="4f06d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f06d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timecards/{timecardID}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f06d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4f06d-119">Optional query parameters</span></span>
<span data-ttu-id="4f06d-120">Este método não dá suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4f06d-120">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f06d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f06d-121">Request headers</span></span>

| <span data-ttu-id="4f06d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f06d-122">Header</span></span>       | <span data-ttu-id="4f06d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4f06d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4f06d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f06d-124">Authorization</span></span>  | <span data-ttu-id="4f06d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f06d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4f06d-127">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="4f06d-127">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="4f06d-128">A ID do usuário em nome do qual o aplicativo está agindo.</span><span class="sxs-lookup"><span data-stu-id="4f06d-128">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="4f06d-129">Obrigatório ao usar o escopo de permissão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f06d-129">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f06d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f06d-130">Request body</span></span>
<span data-ttu-id="4f06d-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f06d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f06d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f06d-132">Response</span></span>

<span data-ttu-id="4f06d-133">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [timeCard](../resources/timeCard.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f06d-133">If successful, this method returns a `200 OK` response code and a [timeCard](../resources/timeCard.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f06d-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f06d-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f06d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f06d-135">Request</span></span>
<span data-ttu-id="4f06d-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f06d-136">The following is an example of the request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="4f06d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f06d-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-get"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972
```
# <a name="c"></a>[<span data-ttu-id="4f06d-138">C#</span><span class="sxs-lookup"><span data-stu-id="4f06d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timecard-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f06d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f06d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f06d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f06d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f06d-141">Java</span><span class="sxs-lookup"><span data-stu-id="4f06d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timecard-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f06d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f06d-142">Response</span></span>

<span data-ttu-id="4f06d-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4f06d-143">The following is an example of the response.</span></span> 

><span data-ttu-id="4f06d-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4f06d-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972",
    "createdDateTime": "2021-05-27T22:58:41.327Z",
    "lastModifiedDateTime": "2021-05-27T23:02:04.187Z",
    "userId": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
    "state": "clockedOut",
    "confirmedBy": "user,manager",
    "notes": null,
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
            "displayName": "Jing Jing GuTwo"
        }
    },
    "clockInEvent": {
        "dateTime": "2021-05-27T22:58:41.327Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "clock in notes"
        }
    },
    "clockOutEvent": {
        "dateTime": "2021-05-27T23:01:46.205Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "clock out smaple notes"
        }
    },
    "breaks": [
        {
            "breakId": "BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f",
            "notes": null,
            "start": {
                "dateTime": "2021-05-27T22:59:59.328Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "start break smaple notes"
                }
            },
            "end": {
                "dateTime": "2021-05-27T23:01:10.205Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "end break smaple notes"
                }
            }
        }
    ],
    "originalEntry": {
        "clockInEvent": {
            "dateTime": "2021-05-27T22:58:41.327Z",
            "atApprovedLocation": null,
            "notes": {
                "contentType": "text",
                "content": "clock in notes"
            }
        },
        "clockOutEvent": {
            "dateTime": "2021-05-27T23:01:46.205Z",
            "atApprovedLocation": null,
            "notes": {
                "contentType": "text",
                "content": "clock out smaple notes"
            }
        },
        "breaks": [
            {
                "breakId": "BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f",
                "notes": null,
                "start": {
                    "dateTime": "2021-05-27T22:59:59.328Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "start break smaple notes"
                    }
                },
                "end": {
                    "dateTime": "2021-05-27T23:01:10.205Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "end break smaple notes"
                    }
                }
            }
        ]
    },
    "createdBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
            "displayName": "Jing Jing GuTwo"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a timeCard by ID",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

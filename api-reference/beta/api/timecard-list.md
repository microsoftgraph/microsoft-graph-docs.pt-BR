---
title: Listar timeCard
description: Recupere uma lista de entradas timeCard na agenda.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1635e8c524b25b3795bf90f03449eddf259ff208
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787835"
---
# <a name="list-timecard"></a><span data-ttu-id="c29f4-103">Listar timeCard</span><span class="sxs-lookup"><span data-stu-id="c29f4-103">List timeCard</span></span>

<span data-ttu-id="c29f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c29f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c29f4-105">Recuperar uma lista de [entradas timeCard](../resources/timecard.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="c29f4-105">Retrieve a list of [timeCard](../resources/timecard.md) entries in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c29f4-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c29f4-106">Permissions</span></span>

<span data-ttu-id="c29f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c29f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c29f4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c29f4-109">Permission type</span></span>      | <span data-ttu-id="c29f4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c29f4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c29f4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c29f4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c29f4-112">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c29f4-112">Schedule.Read.All, Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="c29f4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c29f4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c29f4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c29f4-114">Not supported.</span></span>    |
|<span data-ttu-id="c29f4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c29f4-115">Application</span></span> | <span data-ttu-id="c29f4-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="c29f4-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="c29f4-117">\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.</span><span class="sxs-lookup"><span data-stu-id="c29f4-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="c29f4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c29f4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timecards
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c29f4-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c29f4-119">Optional query parameters</span></span>

<span data-ttu-id="c29f4-120">Este método dá suporte aos parâmetros de consulta `$filter` , , , `$orderBy` `$top` `$skipToken` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c29f4-120">This method supports the `$filter`, `$orderBy`, `$top`, `$skipToken` OData query parameters to help customize the response.</span></span> <span data-ttu-id="c29f4-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c29f4-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c29f4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c29f4-122">Request headers</span></span>

| <span data-ttu-id="c29f4-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c29f4-123">Header</span></span>       | <span data-ttu-id="c29f4-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c29f4-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c29f4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c29f4-125">Authorization</span></span>  | <span data-ttu-id="c29f4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c29f4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c29f4-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="c29f4-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="c29f4-129">A ID do usuário em nome do qual o aplicativo está agindo.</span><span class="sxs-lookup"><span data-stu-id="c29f4-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="c29f4-130">Obrigatório ao usar o escopo de permissão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c29f4-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c29f4-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c29f4-131">Request body</span></span>
<span data-ttu-id="c29f4-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c29f4-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c29f4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c29f4-133">Response</span></span>

<span data-ttu-id="c29f4-134">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma lista de objetos [timeCard](../resources/timeCard.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c29f4-134">If successful, this method returns a `200 OK` response code and a list of [timeCard](../resources/timeCard.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c29f4-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c29f4-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="c29f4-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c29f4-136">Request</span></span>
<span data-ttu-id="c29f4-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c29f4-137">The following is an example of the request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="c29f4-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c29f4-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-list"
}-->

```http
GET https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards?$top=2&$filter=state eq 'clockedOut'

```

### <a name="response"></a><span data-ttu-id="c29f4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c29f4-139">Response</span></span>

<span data-ttu-id="c29f4-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c29f4-140">The following is an example of the response.</span></span> 

><span data-ttu-id="c29f4-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c29f4-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "@odata.etag": "\"3400c313-0000-0d00-0000-60afe1940000\"",
            "id": "TCK_d1e0f245-9996-4125-b128-d3eb5c4b0164",
            "createdDateTime": "2020-09-21T18:01:29.302Z",
            "lastModifiedDateTime": "2021-05-27T18:14:44.503Z",
            "userId": "66b4f2a4-425d-4dec-8172-7e889950885e",
            "state": "clockedOut",
            "confirmedBy": "none",
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
                "dateTime": "2020-09-21T18:01:29.302Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "ClockIn-OBO Shorbani"
                }
            },
            "clockOutEvent": {
                "dateTime": "2021-05-27T18:14:44.503Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "clock out notes"
                }
            },
            "breaks": [],
            "originalEntry": {
                "clockInEvent": {
                    "dateTime": "2020-09-21T18:01:29.302Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "ClockIn-OBO Shorbani"
                    }
                },
                "clockOutEvent": {
                    "dateTime": "2021-05-27T18:14:44.503Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "clock out notes"
                    }
                },
                "breaks": []
            },
            "createdBy": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "66b4f2a4-425d-4dec-8172-7e889950885e",
                    "displayName": "Janani Varadharajan"
                }
            }
        },
        {
            "@odata.etag": "\"3400d914-0000-0d00-0000-60afe1ee0000\"",
            "id": "TCK_aa73c610-dd75-4021-bb5c-6b071c7aa835",
            "createdDateTime": "2020-09-21T18:02:48.688Z",
            "lastModifiedDateTime": "2021-05-27T18:16:14.766Z",
            "userId": "3041ccde-7544-4ae0-b44f-3618b08ba1ce",
            "state": "clockedOut",
            "confirmedBy": "none",
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
                "dateTime": "2020-09-21T18:02:48.688Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "ClockIn-OBO Shorbani"
                }
            },
            "clockOutEvent": {
                "dateTime": "2021-05-27T18:16:14.766Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "clock out notes"
                }
            },
            "breaks": [],
            "originalEntry": {
                "clockInEvent": {
                    "dateTime": "2020-09-21T18:02:48.688Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "ClockIn-OBO Shorbani"
                    }
                },
                "clockOutEvent": {
                    "dateTime": "2021-05-27T18:16:14.766Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "clock out notes"
                    }
                },
                "breaks": []
            },
            "createdBy": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "66b4f2a4-425d-4dec-8172-7e889950885e",
                    "displayName": "Janani Varadharajan"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Retrieve a list of timeCard entries in the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

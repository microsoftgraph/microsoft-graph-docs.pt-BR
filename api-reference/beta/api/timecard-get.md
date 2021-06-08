---
title: Obter timeCard
description: Obter um cartão de ponto por ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f1e2424a9303caa69aa2f64798f9c61388418723
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787836"
---
# <a name="get-timecard"></a><span data-ttu-id="7516a-103">Obter timeCard</span><span class="sxs-lookup"><span data-stu-id="7516a-103">Get timeCard</span></span>

<span data-ttu-id="7516a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7516a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7516a-105">Recupere as propriedades e as relações de um [objeto timeCard](../resources/timeCard.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="7516a-105">Retrieve the properties and relationships of a [timeCard](../resources/timeCard.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="7516a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7516a-106">Permissions</span></span>

<span data-ttu-id="7516a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7516a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7516a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7516a-109">Permission type</span></span>      | <span data-ttu-id="7516a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7516a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7516a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7516a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7516a-112">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7516a-112">Schedule.Read.All, Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="7516a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7516a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7516a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7516a-114">Not supported.</span></span>    |
|<span data-ttu-id="7516a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7516a-115">Application</span></span> | <span data-ttu-id="7516a-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="7516a-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="7516a-117">\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.</span><span class="sxs-lookup"><span data-stu-id="7516a-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="7516a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7516a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timecards/{timecardID}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="7516a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7516a-119">Optional query parameters</span></span>
<span data-ttu-id="7516a-120">Este método não dá suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7516a-120">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7516a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7516a-121">Request headers</span></span>

| <span data-ttu-id="7516a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7516a-122">Header</span></span>       | <span data-ttu-id="7516a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7516a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7516a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7516a-124">Authorization</span></span>  | <span data-ttu-id="7516a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7516a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7516a-127">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="7516a-127">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="7516a-128">A ID do usuário em nome do qual o aplicativo está agindo.</span><span class="sxs-lookup"><span data-stu-id="7516a-128">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="7516a-129">Obrigatório ao usar o escopo de permissão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7516a-129">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7516a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7516a-130">Request body</span></span>
<span data-ttu-id="7516a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7516a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7516a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7516a-132">Response</span></span>

<span data-ttu-id="7516a-133">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [timeCard](../resources/timeCard.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7516a-133">If successful, this method returns a `200 OK` response code and a [timeCard](../resources/timeCard.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7516a-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7516a-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="7516a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7516a-135">Request</span></span>
<span data-ttu-id="7516a-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7516a-136">The following is an example of the request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="7516a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7516a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-get"
}-->

```http
GET https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972
```

### <a name="response"></a><span data-ttu-id="7516a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7516a-138">Response</span></span>

<span data-ttu-id="7516a-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7516a-139">The following is an example of the response.</span></span> 

><span data-ttu-id="7516a-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7516a-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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

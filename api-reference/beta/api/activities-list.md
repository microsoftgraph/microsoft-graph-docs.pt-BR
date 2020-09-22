---
author: daspek
ms.author: dspektor
ms.date: 09/10/2017
title: Atividades de arquivo
description: Lista as atividades recentes que foram realizadas em um item ou em uma hierarquia.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: e75043fe3d91754902b078d6bd88b1227295587a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983435"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="ee0d2-103">Enumerar atividades (prévia)</span><span class="sxs-lookup"><span data-stu-id="ee0d2-103">Enumerate activities (preview)</span></span>

<span data-ttu-id="ee0d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee0d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee0d2-105">Lista as [atividades](../resources/itemactivity.md) recentes que foram realizadas em um item ou em uma hierarquia.</span><span class="sxs-lookup"><span data-stu-id="ee0d2-105">List the recent [activities](../resources/itemactivity.md) that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="ee0d2-106">**Observação:** as atividades são uma Visualização limitada e ainda não disponível para todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="ee0d2-106">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="ee0d2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee0d2-107">Permissions</span></span>

<span data-ttu-id="ee0d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee0d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee0d2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee0d2-110">Permission type</span></span>                        | <span data-ttu-id="ee0d2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee0d2-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="ee0d2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee0d2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee0d2-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee0d2-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="ee0d2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee0d2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee0d2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee0d2-115">Not supported.</span></span>
|<span data-ttu-id="ee0d2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee0d2-116">Application</span></span>                            | <span data-ttu-id="ee0d2-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee0d2-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="ee0d2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee0d2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="ee0d2-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee0d2-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ee0d2-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee0d2-120">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ee0d2-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee0d2-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-activities" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/activities
```
# <a name="c"></a>[<span data-ttu-id="ee0d2-122">C#</span><span class="sxs-lookup"><span data-stu-id="ee0d2-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-activities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee0d2-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee0d2-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-activities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee0d2-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee0d2-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-activities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ee0d2-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee0d2-125">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivity)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "action": {
                "comment": {}
            },
            "actor": {
                "user": {
                    "displayName": "Xavier Wilke"
                }
            },
            "id": "EJalEvjV1EgIYFQAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-29T18:34:40Z"
            }
        },
        {
            "action": {
                "edit": {},
                "version": {
                    "newVersion": "2.0"
                }
            },
            "actor": {
                "user": {
                    "displayName": "Judith Clemons"
                }
            },
            "id": "cInT6/fV1EgFYFQAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-29T16:23:35Z"
            }
        },
        {
            "action": {
                "mention": {
                    "mentionees": [
                        {
                            "user": {
                                "displayName": "Judith Clemons"
                            }
                        }
                    ]
                }
            },
            "actor": {
                "user": {
                    "displayName": "Misty Suarez"
                }
            },
            "id": "EBJa0vPV1EjFX1QAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-28T20:14:14Z"
            }
        },
        {
            "action": {
                "rename": {
                    "oldName": "Document2.docx"
                }
            },
            "actor": {
                "user": {
                    "displayName": "Misty Suarez"
                }
            },
            "id": "QFJFlfPV1Ei/X1QAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-28T20:12:32Z"
            }
        },
        {
            "action": {
                "create": {}
            },
            "actor": {
                "user": {
                    "displayName": "Misty Suarez"
                }
            },
            "id": "IJydkPPV1Ei9X1QAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-28T20:02:24Z"
            }
        }
    ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
  ]
}
-->



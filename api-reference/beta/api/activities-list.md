---
author: daspek
ms.author: dspektor
ms.date: 09/10/2017
title: Atividades de arquivo
localization_priority: Normal
ms.openlocfilehash: 87b46648f59f0b6c4f50390bd510edf54758af82
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636720"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="bf73d-102">Enumerar atividades (prévia)</span><span class="sxs-lookup"><span data-stu-id="bf73d-102">Enumerate activities (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf73d-103">Lista as [atividades](../resources/itemactivity.md) recentes que foram realizadas em um item ou em uma hierarquia.</span><span class="sxs-lookup"><span data-stu-id="bf73d-103">List the recent [activities](../resources/itemactivity.md) that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="bf73d-104">**Observação:** as atividades são uma Visualização limitada e ainda não disponível para todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="bf73d-104">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="bf73d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf73d-105">Permissions</span></span>

<span data-ttu-id="bf73d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf73d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf73d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf73d-108">Permission type</span></span>                        | <span data-ttu-id="bf73d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf73d-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="bf73d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf73d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bf73d-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf73d-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="bf73d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf73d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf73d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf73d-113">Not supported.</span></span>
|<span data-ttu-id="bf73d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf73d-114">Application</span></span>                            | <span data-ttu-id="bf73d-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf73d-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="bf73d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf73d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="bf73d-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf73d-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bf73d-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf73d-118">Request</span></span>

<!-- { "blockType": "request", "name": "list-activities" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/activities
```

#### <a name="response"></a><span data-ttu-id="bf73d-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf73d-119">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="bf73d-120">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="bf73d-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bf73d-121">Basic</span><span class="sxs-lookup"><span data-stu-id="bf73d-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list-activities-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bf73d-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf73d-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list-activities-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
    "Error: /api-reference/beta/api/activities-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/activities-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

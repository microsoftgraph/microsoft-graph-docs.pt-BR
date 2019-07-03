---
author: daspek
ms.author: dspektor
ms.date: 09/10/2017
title: Atividades de arquivo
localization_priority: Normal
ms.openlocfilehash: 223a171e4da8ec009060d2e3a5f8f1f93d300007
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439970"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="7dc96-102">Enumerar atividades (prévia)</span><span class="sxs-lookup"><span data-stu-id="7dc96-102">Enumerate activities (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dc96-103">Lista as [atividades](../resources/itemactivity.md) recentes que foram realizadas em um item ou em uma hierarquia.</span><span class="sxs-lookup"><span data-stu-id="7dc96-103">List the recent [activities](../resources/itemactivity.md) that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="7dc96-104">**Observação:** as atividades são uma Visualização limitada e ainda não disponível para todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="7dc96-104">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="7dc96-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7dc96-105">Permissions</span></span>

<span data-ttu-id="7dc96-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dc96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dc96-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7dc96-108">Permission type</span></span>                        | <span data-ttu-id="7dc96-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7dc96-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="7dc96-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7dc96-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7dc96-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dc96-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="7dc96-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7dc96-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dc96-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dc96-113">Not supported.</span></span>
|<span data-ttu-id="7dc96-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7dc96-114">Application</span></span>                            | <span data-ttu-id="7dc96-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dc96-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="7dc96-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7dc96-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="7dc96-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7dc96-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7dc96-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7dc96-118">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7dc96-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dc96-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-activities" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/activities
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7dc96-120">C#</span><span class="sxs-lookup"><span data-stu-id="7dc96-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-activities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7dc96-121">Javascript</span><span class="sxs-lookup"><span data-stu-id="7dc96-121">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-activities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7dc96-122">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7dc96-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-activities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7dc96-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dc96-123">Response</span></span>

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

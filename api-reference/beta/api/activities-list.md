---
author: daspek
ms.author: dspektor
ms.date: 09/10/2017
title: Atividades de arquivo
ms.openlocfilehash: f228f96083d899c4d9a43f6a4d41f2b90ce2eaf7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034342"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="5f72e-102">Enumerar atividades (prévia)</span><span class="sxs-lookup"><span data-stu-id="5f72e-102">Enumerate activities (preview)</span></span>

> <span data-ttu-id="5f72e-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5f72e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f72e-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5f72e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f72e-105">Lista as [atividades][] recentes que foram realizadas em um item ou em uma hierarquia.</span><span class="sxs-lookup"><span data-stu-id="5f72e-105">List the recent [activities][] that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="5f72e-106">**Observação:** as atividades são uma Visualização limitada e ainda não disponível para todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="5f72e-106">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[atividades]: ../resources/itemactivity.md
[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="5f72e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f72e-108">Permissions</span></span>

<span data-ttu-id="5f72e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f72e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f72e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f72e-111">Permission type</span></span>                        | <span data-ttu-id="5f72e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f72e-112">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="5f72e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f72e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f72e-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f72e-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="5f72e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f72e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f72e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f72e-116">Not supported.</span></span>
|<span data-ttu-id="5f72e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f72e-117">Application</span></span>                            | <span data-ttu-id="5f72e-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f72e-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="5f72e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f72e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="5f72e-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f72e-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5f72e-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f72e-121">Request</span></span>

<!-- { "blockType": "request", "name": "list-activities" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/activities
```

#### <a name="response"></a><span data-ttu-id="5f72e-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f72e-122">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites"
} -->

---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Obtenha a análise
ms.openlocfilehash: 57f009e0d2a07a5bf8c9a0f3b3617083bc279545
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037397"
---
# <a name="get-analytics"></a><span data-ttu-id="b543f-102">Obtenha a análise</span><span class="sxs-lookup"><span data-stu-id="b543f-102">Get analytics</span></span>

> <span data-ttu-id="b543f-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b543f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b543f-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b543f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b543f-105">Obtenha [itemAnalytics][] sobre os modos de exibição que foi realizada sob este recurso.</span><span class="sxs-lookup"><span data-stu-id="b543f-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="b543f-106">O recurso de **itemAnalytics** é uma maneira conveniente para obter as estatísticas de atividade do `allTime` e o `lastSevenDays`.</span><span class="sxs-lookup"><span data-stu-id="b543f-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="b543f-107">Para um intervalo de tempo personalizado ou um intervalo, use o [getActivitiesByInterval][] API.</span><span class="sxs-lookup"><span data-stu-id="b543f-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="b543f-108">**Observação:** O recurso de **itemAnalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="b543f-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="b543f-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="b543f-111">Permissions</span></span>

<span data-ttu-id="b543f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b543f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b543f-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b543f-114">Permission type</span></span>                        | <span data-ttu-id="b543f-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b543f-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="b543f-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b543f-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="b543f-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b543f-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="b543f-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b543f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b543f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b543f-119">Not supported.</span></span>
|<span data-ttu-id="b543f-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b543f-120">Application</span></span>                            | <span data-ttu-id="b543f-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b543f-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="b543f-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b543f-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="b543f-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b543f-123">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b543f-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b543f-124">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

#### <a name="response"></a><span data-ttu-id="b543f-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b543f-125">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "allTime": {
        "access": {
            "actionCount": 123,
            "actorCount": 89
        }
    },
    "lastSevenDays": {
        "access": {
            "actionCount": 52,
            "actorCount": 41
        }
    }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics"
} -->

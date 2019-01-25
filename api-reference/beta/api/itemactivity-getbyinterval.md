---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Obter estatísticas de atividade de item pelo intervalo
localization_priority: Normal
ms.openlocfilehash: f9601538d825efe346ab57fdbecd6c74dc9978d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516452"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="2f008-102">Obter estatísticas de atividade de item pelo intervalo</span><span class="sxs-lookup"><span data-stu-id="2f008-102">Get item activity stats by interval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f008-103">Obtenha [itemActivityStats][] para as atividades que foram realizada sob este recurso dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="2f008-103">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="2f008-104">**Observação:** O recurso de **itemAnalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="2f008-104">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="2f008-105">Agregações da análise não podem estar disponíveis para todos os tipos de ação.</span><span class="sxs-lookup"><span data-stu-id="2f008-105">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="2f008-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f008-107">Permissions</span></span>

<span data-ttu-id="2f008-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f008-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f008-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f008-110">Permission type</span></span>                        | <span data-ttu-id="2f008-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f008-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="2f008-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f008-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f008-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f008-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="2f008-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f008-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f008-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f008-115">Not supported.</span></span>
|<span data-ttu-id="2f008-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f008-116">Application</span></span>                            | <span data-ttu-id="2f008-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f008-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="2f008-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f008-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="2f008-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="2f008-119">Function parameters</span></span>

| <span data-ttu-id="2f008-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2f008-120">Parameter</span></span>      | <span data-ttu-id="2f008-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f008-121">Type</span></span>               | <span data-ttu-id="2f008-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f008-122">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="2f008-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2f008-123">startDateTime</span></span>  | <span data-ttu-id="2f008-124">cadeia de caracteres (timestamp)</span><span class="sxs-lookup"><span data-stu-id="2f008-124">string (timestamp)</span></span> | <span data-ttu-id="2f008-125">A hora de início através do qual a atividades de agregação.</span><span class="sxs-lookup"><span data-stu-id="2f008-125">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="2f008-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2f008-126">endDateTime</span></span>    | <span data-ttu-id="2f008-127">cadeia de caracteres (timestamp)</span><span class="sxs-lookup"><span data-stu-id="2f008-127">string (timestamp)</span></span> | <span data-ttu-id="2f008-128">A hora de término através do qual a atividades de agregação.</span><span class="sxs-lookup"><span data-stu-id="2f008-128">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="2f008-129">interval</span><span class="sxs-lookup"><span data-stu-id="2f008-129">interval</span></span>       | <span data-ttu-id="2f008-130">string</span><span class="sxs-lookup"><span data-stu-id="2f008-130">string</span></span>             | <span data-ttu-id="2f008-131">O intervalo de agregação de lista segura.</span><span class="sxs-lookup"><span data-stu-id="2f008-131">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="2f008-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f008-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2f008-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f008-133">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a><span data-ttu-id="2f008-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f008-134">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivityStat)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "startDateTime": "2017-01-01T00:00:00.000Z",
            "endDateTime": "2017-01-02T00:00:00.000Z",
            "delete": {
                "actionCount": 1,
                "actorCount": 1
            },
            "access": {
                "actionCount": 5,
                "actorCount": 3
            }
        },
        {
            "startDateTime": "2017-01-02T00:00:00.000Z",
            "endDateTime": "2017-01-03T00:00:00.000Z",
            "edit": {
                "actionCount": 3,
                "actorCount": 1
            },
            "access": {
                "actionCount": 7,
                "actorCount": 6
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
  "tocPath": "BaseItem/Get activities by interval",
  "suppressions": [
    "Error: /api-reference/beta/api/itemactivity-getbyinterval.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Obter estatísticas de atividade de item por intervalo
localization_priority: Normal
ms.openlocfilehash: f9601538d825efe346ab57fdbecd6c74dc9978d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541296"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="b46bf-102">Obter estatísticas de atividade de item por intervalo</span><span class="sxs-lookup"><span data-stu-id="b46bf-102">Get item activity stats by interval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b46bf-103">Obter [itemActivityStats][] para as atividades que foram realizadas sob esse recurso dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="b46bf-103">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="b46bf-104">**Observação:** O \*\*\*\* recurso do naanalytics ainda não está disponível em todas as implantações [nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="b46bf-104">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="b46bf-105">As agregações de análise podem não estar disponíveis para todos os tipos de ação.</span><span class="sxs-lookup"><span data-stu-id="b46bf-105">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="b46bf-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b46bf-107">Permissions</span></span>

<span data-ttu-id="b46bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b46bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b46bf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b46bf-110">Permission type</span></span>                        | <span data-ttu-id="b46bf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b46bf-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="b46bf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b46bf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b46bf-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b46bf-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="b46bf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b46bf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b46bf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b46bf-115">Not supported.</span></span>
|<span data-ttu-id="b46bf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b46bf-116">Application</span></span>                            | <span data-ttu-id="b46bf-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b46bf-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="b46bf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b46bf-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="b46bf-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b46bf-119">Function parameters</span></span>

| <span data-ttu-id="b46bf-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b46bf-120">Parameter</span></span>      | <span data-ttu-id="b46bf-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b46bf-121">Type</span></span>               | <span data-ttu-id="b46bf-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b46bf-122">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="b46bf-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b46bf-123">startDateTime</span></span>  | <span data-ttu-id="b46bf-124">Cadeia de caracteres (timestamp)</span><span class="sxs-lookup"><span data-stu-id="b46bf-124">string (timestamp)</span></span> | <span data-ttu-id="b46bf-125">A hora de início em que as atividades serão agregadas.</span><span class="sxs-lookup"><span data-stu-id="b46bf-125">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="b46bf-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b46bf-126">endDateTime</span></span>    | <span data-ttu-id="b46bf-127">Cadeia de caracteres (timestamp)</span><span class="sxs-lookup"><span data-stu-id="b46bf-127">string (timestamp)</span></span> | <span data-ttu-id="b46bf-128">A hora de término sobre a qual agregar atividades.</span><span class="sxs-lookup"><span data-stu-id="b46bf-128">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="b46bf-129">interval</span><span class="sxs-lookup"><span data-stu-id="b46bf-129">interval</span></span>       | <span data-ttu-id="b46bf-130">string</span><span class="sxs-lookup"><span data-stu-id="b46bf-130">string</span></span>             | <span data-ttu-id="b46bf-131">O intervalo de agregação.</span><span class="sxs-lookup"><span data-stu-id="b46bf-131">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="b46bf-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b46bf-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b46bf-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b46bf-133">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a><span data-ttu-id="b46bf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b46bf-134">Response</span></span>

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

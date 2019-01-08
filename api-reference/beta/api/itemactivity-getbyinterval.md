---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Obter estatísticas de atividade de item pelo intervalo
ms.openlocfilehash: 3b3c7139678715a11365f2551c318dcf66e68e7a
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748187"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="39675-102">Obter estatísticas de atividade de item pelo intervalo</span><span class="sxs-lookup"><span data-stu-id="39675-102">Get item activity stats by interval</span></span>

> <span data-ttu-id="39675-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="39675-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39675-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="39675-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="39675-105">Obtenha [itemActivityStats][] para as atividades que foram realizada sob este recurso dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="39675-105">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="39675-106">**Observação:** O recurso de **itemAnalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="39675-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="39675-107">Agregações da análise não podem estar disponíveis para todos os tipos de ação.</span><span class="sxs-lookup"><span data-stu-id="39675-107">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="39675-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="39675-109">Permissions</span></span>

<span data-ttu-id="39675-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39675-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39675-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39675-112">Permission type</span></span>                        | <span data-ttu-id="39675-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39675-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="39675-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39675-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="39675-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39675-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="39675-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39675-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39675-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39675-117">Not supported.</span></span>
|<span data-ttu-id="39675-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39675-118">Application</span></span>                            | <span data-ttu-id="39675-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39675-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="39675-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39675-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="39675-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="39675-121">Function parameters</span></span>

| <span data-ttu-id="39675-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="39675-122">Parameter</span></span>      | <span data-ttu-id="39675-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="39675-123">Type</span></span>               | <span data-ttu-id="39675-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="39675-124">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="39675-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="39675-125">startDateTime</span></span>  | <span data-ttu-id="39675-126">cadeia de caracteres (timestamp)</span><span class="sxs-lookup"><span data-stu-id="39675-126">string (timestamp)</span></span> | <span data-ttu-id="39675-127">A hora de início através do qual a atividades de agregação.</span><span class="sxs-lookup"><span data-stu-id="39675-127">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="39675-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="39675-128">endDateTime</span></span>    | <span data-ttu-id="39675-129">cadeia de caracteres (timestamp)</span><span class="sxs-lookup"><span data-stu-id="39675-129">string (timestamp)</span></span> | <span data-ttu-id="39675-130">A hora de término através do qual a atividades de agregação.</span><span class="sxs-lookup"><span data-stu-id="39675-130">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="39675-131">interval</span><span class="sxs-lookup"><span data-stu-id="39675-131">interval</span></span>       | <span data-ttu-id="39675-132">string</span><span class="sxs-lookup"><span data-stu-id="39675-132">string</span></span>             | <span data-ttu-id="39675-133">O intervalo de agregação de lista segura.</span><span class="sxs-lookup"><span data-stu-id="39675-133">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="39675-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39675-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="39675-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39675-135">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a><span data-ttu-id="39675-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="39675-136">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get activities by interval"
} -->

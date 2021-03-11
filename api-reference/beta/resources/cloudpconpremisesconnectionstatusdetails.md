---
title: Tipo de recurso cloudPcOnPremisesConnectionStatusDetails
description: Os detalhes de status de uma conexão local do computador na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7ef9847190fb851482d29535d0709f3d74bbf3aa
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722171"
---
# <a name="cloudpconpremisesconnectionstatusdetails-resource-type"></a><span data-ttu-id="ba2cf-103">Tipo de recurso cloudPcOnPremisesConnectionStatusDetails</span><span class="sxs-lookup"><span data-stu-id="ba2cf-103">cloudPcOnPremisesConnectionStatusDetails resource type</span></span>

<span data-ttu-id="ba2cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba2cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba2cf-105">Os detalhes de status de [um cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="ba2cf-105">The status details of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="ba2cf-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba2cf-106">Properties</span></span>

|<span data-ttu-id="ba2cf-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba2cf-107">Property</span></span>|<span data-ttu-id="ba2cf-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba2cf-108">Type</span></span>|<span data-ttu-id="ba2cf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba2cf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba2cf-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ba2cf-110">startDateTime</span></span>|<span data-ttu-id="ba2cf-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba2cf-111">DateTimeOffset</span></span>|<span data-ttu-id="ba2cf-112">A hora de início da verificação de saúde da conexão.</span><span class="sxs-lookup"><span data-stu-id="ba2cf-112">The start time of the connection health check.</span></span> <span data-ttu-id="ba2cf-113">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ba2cf-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ba2cf-114">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="ba2cf-114">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="ba2cf-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ba2cf-115">endDateTime</span></span>|<span data-ttu-id="ba2cf-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba2cf-116">DateTimeOffset</span></span>|<span data-ttu-id="ba2cf-117">A hora de término da verificação de saúde da conexão.</span><span class="sxs-lookup"><span data-stu-id="ba2cf-117">The end time of the connection health check.</span></span> <span data-ttu-id="ba2cf-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ba2cf-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ba2cf-119">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="ba2cf-119">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="ba2cf-120">healthChecks</span><span class="sxs-lookup"><span data-stu-id="ba2cf-120">healthChecks</span></span>|<span data-ttu-id="ba2cf-121">[coleção cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md)</span><span class="sxs-lookup"><span data-stu-id="ba2cf-121">[cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md) collection</span></span>|<span data-ttu-id="ba2cf-122">Todas as verificações feitas na conexão.</span><span class="sxs-lookup"><span data-stu-id="ba2cf-122">All checks that are done on the connection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba2cf-123">Relações</span><span class="sxs-lookup"><span data-stu-id="ba2cf-123">Relationships</span></span>

<span data-ttu-id="ba2cf-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba2cf-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba2cf-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba2cf-125">JSON representation</span></span>

<span data-ttu-id="ba2cf-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba2cf-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionStatusDetails"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnectionStatusDetails",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "healthChecks": [
    {
      "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
      "displayName": "String",
      "status": "String",
      "startDateTime": "String (timestamp)",
      "endDateTime": "String (timestamp)",
      "errorType": "String",
      "recommendedAction": "String",
      "additionalDetails": "String"
    }
  ]
}
```

---
title: tipo de recurso cloudPcOnPremisesConnectionStatusDetails
description: Os detalhes de status de uma conexão local do PC de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: db40df3bcd89ac21eb50870e82fe6a34ced86828
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563769"
---
# <a name="cloudpconpremisesconnectionstatusdetails-resource-type"></a><span data-ttu-id="d6538-103">tipo de recurso cloudPcOnPremisesConnectionStatusDetails</span><span class="sxs-lookup"><span data-stu-id="d6538-103">cloudPcOnPremisesConnectionStatusDetails resource type</span></span>

<span data-ttu-id="d6538-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6538-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6538-105">Os detalhes de status de um [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="d6538-105">The status details of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="d6538-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6538-106">Properties</span></span>

|<span data-ttu-id="d6538-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6538-107">Property</span></span>|<span data-ttu-id="d6538-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6538-108">Type</span></span>|<span data-ttu-id="d6538-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6538-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6538-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d6538-110">startDateTime</span></span>|<span data-ttu-id="d6538-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6538-111">DateTimeOffset</span></span>|<span data-ttu-id="d6538-112">A hora de início da verificação de integridade da conexão.</span><span class="sxs-lookup"><span data-stu-id="d6538-112">The start time of the connection health check.</span></span> <span data-ttu-id="d6538-113">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d6538-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d6538-114">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="d6538-114">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="d6538-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d6538-115">endDateTime</span></span>|<span data-ttu-id="d6538-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6538-116">DateTimeOffset</span></span>|<span data-ttu-id="d6538-117">A hora de término da verificação de integridade da conexão.</span><span class="sxs-lookup"><span data-stu-id="d6538-117">The end time of the connection health check.</span></span> <span data-ttu-id="d6538-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d6538-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d6538-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="d6538-119">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="d6538-120">healthChecks</span><span class="sxs-lookup"><span data-stu-id="d6538-120">healthChecks</span></span>|<span data-ttu-id="d6538-121">coleção [cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md)</span><span class="sxs-lookup"><span data-stu-id="d6538-121">[cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md) collection</span></span>|<span data-ttu-id="d6538-122">Todas as verificações realizadas na conexão.</span><span class="sxs-lookup"><span data-stu-id="d6538-122">All checks that are done on the connection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6538-123">Relações</span><span class="sxs-lookup"><span data-stu-id="d6538-123">Relationships</span></span>

<span data-ttu-id="d6538-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6538-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6538-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6538-125">JSON representation</span></span>

<span data-ttu-id="d6538-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6538-126">The following is a JSON representation of the resource.</span></span>
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

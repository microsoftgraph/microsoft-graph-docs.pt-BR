---
title: tipo de recurso cloudPcOnPremisesConnectionStatusDetails
description: Os detalhes de status de uma conexão local do PC de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 19dedd3344d5ed049a5b6ff5361ed7a8e4937146
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378206"
---
# <a name="cloudpconpremisesconnectionstatusdetails-resource-type"></a><span data-ttu-id="abcd3-103">tipo de recurso cloudPcOnPremisesConnectionStatusDetails</span><span class="sxs-lookup"><span data-stu-id="abcd3-103">cloudPcOnPremisesConnectionStatusDetails resource type</span></span>

<span data-ttu-id="abcd3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abcd3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="abcd3-105">Os detalhes de status de um [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="abcd3-105">The status details of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="abcd3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="abcd3-106">Properties</span></span>

|<span data-ttu-id="abcd3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abcd3-107">Property</span></span>|<span data-ttu-id="abcd3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="abcd3-108">Type</span></span>|<span data-ttu-id="abcd3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="abcd3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abcd3-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="abcd3-110">startDateTime</span></span>|<span data-ttu-id="abcd3-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abcd3-111">DateTimeOffset</span></span>|<span data-ttu-id="abcd3-112">A hora de início da verificação de integridade da conexão.</span><span class="sxs-lookup"><span data-stu-id="abcd3-112">The start time of the connection health check.</span></span> <span data-ttu-id="abcd3-113">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="abcd3-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="abcd3-114">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="abcd3-114">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="abcd3-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="abcd3-115">endDateTime</span></span>|<span data-ttu-id="abcd3-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abcd3-116">DateTimeOffset</span></span>|<span data-ttu-id="abcd3-117">A hora de término da verificação de integridade da conexão.</span><span class="sxs-lookup"><span data-stu-id="abcd3-117">The end time of the connection health check.</span></span> <span data-ttu-id="abcd3-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="abcd3-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="abcd3-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="abcd3-119">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="abcd3-120">healthChecks</span><span class="sxs-lookup"><span data-stu-id="abcd3-120">healthChecks</span></span>|<span data-ttu-id="abcd3-121">coleção [cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md)</span><span class="sxs-lookup"><span data-stu-id="abcd3-121">[cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md) collection</span></span>|<span data-ttu-id="abcd3-122">Todas as verificações realizadas na conexão.</span><span class="sxs-lookup"><span data-stu-id="abcd3-122">All checks that are done on the connection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="abcd3-123">Relações</span><span class="sxs-lookup"><span data-stu-id="abcd3-123">Relationships</span></span>

<span data-ttu-id="abcd3-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="abcd3-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="abcd3-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="abcd3-125">JSON representation</span></span>

<span data-ttu-id="abcd3-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="abcd3-126">The following is a JSON representation of the resource.</span></span>
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

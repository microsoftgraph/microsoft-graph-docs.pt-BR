---
title: tipo de recurso comanagementEligibleDevicesSummary
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b67734bf98a48c31a1346bd730c8521fd8a8d681
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060766"
---
# <a name="comanagementeligibledevicessummary-resource-type"></a><span data-ttu-id="7fde3-103">tipo de recurso comanagementEligibleDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="7fde3-103">comanagementEligibleDevicesSummary resource type</span></span>

<span data-ttu-id="7fde3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fde3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7fde3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7fde3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fde3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7fde3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fde3-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7fde3-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7fde3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7fde3-108">Properties</span></span>
|<span data-ttu-id="7fde3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7fde3-109">Property</span></span>|<span data-ttu-id="7fde3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7fde3-110">Type</span></span>|<span data-ttu-id="7fde3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fde3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fde3-112">comanagedCount</span><span class="sxs-lookup"><span data-stu-id="7fde3-112">comanagedCount</span></span>|<span data-ttu-id="7fde3-113">Int32</span><span class="sxs-lookup"><span data-stu-id="7fde3-113">Int32</span></span>|<span data-ttu-id="7fde3-114">Contagem de dispositivos já cogerenciados</span><span class="sxs-lookup"><span data-stu-id="7fde3-114">Count of devices already Co-Managed</span></span>|
|<span data-ttu-id="7fde3-115">eligibleCount</span><span class="sxs-lookup"><span data-stu-id="7fde3-115">eligibleCount</span></span>|<span data-ttu-id="7fde3-116">Int32</span><span class="sxs-lookup"><span data-stu-id="7fde3-116">Int32</span></span>|<span data-ttu-id="7fde3-117">Contagem de dispositivos totalmente qualificados para o cogerenciamento</span><span class="sxs-lookup"><span data-stu-id="7fde3-117">Count of devices fully eligible for Co-Management</span></span>|
|<span data-ttu-id="7fde3-118">eligibleButNotAzureAdJoinedCount</span><span class="sxs-lookup"><span data-stu-id="7fde3-118">eligibleButNotAzureAdJoinedCount</span></span>|<span data-ttu-id="7fde3-119">Int32</span><span class="sxs-lookup"><span data-stu-id="7fde3-119">Int32</span></span>|<span data-ttu-id="7fde3-120">Contagem de dispositivos qualificados para cogerenciamento, mas ainda não ingressou no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="7fde3-120">Count of devices eligible for Co-Management but not yet joined to Azure Active Directory</span></span>|
|<span data-ttu-id="7fde3-121">needsOsUpdateCount</span><span class="sxs-lookup"><span data-stu-id="7fde3-121">needsOsUpdateCount</span></span>|<span data-ttu-id="7fde3-122">Int32</span><span class="sxs-lookup"><span data-stu-id="7fde3-122">Int32</span></span>|<span data-ttu-id="7fde3-123">Contagem de dispositivos que serão qualificados para cogerenciamento após uma atualização de so</span><span class="sxs-lookup"><span data-stu-id="7fde3-123">Count of devices that will be eligible for Co-Management after an OS update</span></span>|
|<span data-ttu-id="7fde3-124">ineligibleCount</span><span class="sxs-lookup"><span data-stu-id="7fde3-124">ineligibleCount</span></span>|<span data-ttu-id="7fde3-125">Int32</span><span class="sxs-lookup"><span data-stu-id="7fde3-125">Int32</span></span>|<span data-ttu-id="7fde3-126">Contagem de dispositivos não qualificados para cogerenciamento</span><span class="sxs-lookup"><span data-stu-id="7fde3-126">Count of devices ineligible for Co-Management</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fde3-127">Relações</span><span class="sxs-lookup"><span data-stu-id="7fde3-127">Relationships</span></span>
<span data-ttu-id="7fde3-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7fde3-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7fde3-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7fde3-129">JSON Representation</span></span>
<span data-ttu-id="7fde3-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7fde3-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagementEligibleDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevicesSummary",
  "comanagedCount": 1024,
  "eligibleCount": 1024,
  "eligibleButNotAzureAdJoinedCount": 1024,
  "needsOsUpdateCount": 1024,
  "ineligibleCount": 1024
}
```







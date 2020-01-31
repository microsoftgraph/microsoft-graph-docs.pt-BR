---
title: tipo de recurso comanagementEligibleSummaryEntity
description: tipo de recurso comanagementEligibleSummaryEntity
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 80c2afff56d845097990ef927a743678a248c9fd
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636578"
---
# <a name="comanagementeligiblesummaryentity-resource-type"></a><span data-ttu-id="4ad2e-103">tipo de recurso comanagementEligibleSummaryEntity</span><span class="sxs-lookup"><span data-stu-id="4ad2e-103">comanagementEligibleSummaryEntity resource type</span></span>

> <span data-ttu-id="4ad2e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ad2e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ad2e-106">Estado da configuração do aplicativo móvel do dispositivo gerenciado para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-106">Managed Device Mobile App Configuration State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="4ad2e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4ad2e-107">Methods</span></span>
|<span data-ttu-id="4ad2e-108">Método</span><span class="sxs-lookup"><span data-stu-id="4ad2e-108">Method</span></span>|<span data-ttu-id="4ad2e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4ad2e-109">Return Type</span></span>|<span data-ttu-id="4ad2e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ad2e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4ad2e-111">Listar comanagementEligibleSummaryEntity</span><span class="sxs-lookup"><span data-stu-id="4ad2e-111">List comanagementEligibleSummaryEntity</span></span>](../api/intune-device-comanagementEligibleSummaryEntity-list.md)|<span data-ttu-id="4ad2e-112">coleção comanagementEligibleSummaryEntity</span><span class="sxs-lookup"><span data-stu-id="4ad2e-112">comanagementEligibleSummaryEntity collection</span></span>|<span data-ttu-id="4ad2e-113">Listar Propriedades e relações dos objetos comanagementEligibleSummaryEntity.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-113">List properties and relationships of the comanagementEligibleSummaryEntity objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="4ad2e-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ad2e-114">Properties</span></span>
|<span data-ttu-id="4ad2e-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ad2e-115">Property</span></span>|<span data-ttu-id="4ad2e-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ad2e-116">Type</span></span>|<span data-ttu-id="4ad2e-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ad2e-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ad2e-118">id</span><span class="sxs-lookup"><span data-stu-id="4ad2e-118">id</span></span>|<span data-ttu-id="4ad2e-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ad2e-119">String</span></span>|<span data-ttu-id="4ad2e-120">ID exclusiva do EligibleDeviceSummaryEntity</span><span class="sxs-lookup"><span data-stu-id="4ad2e-120">Unique Id of the EligibleDeviceSummaryEntity</span></span>|
|<span data-ttu-id="4ad2e-121">coManagedCount</span><span class="sxs-lookup"><span data-stu-id="4ad2e-121">coManagedCount</span></span>|<span data-ttu-id="4ad2e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="4ad2e-122">Int32</span></span>|<span data-ttu-id="4ad2e-123">Contagem de dispositivos já cogerenciados</span><span class="sxs-lookup"><span data-stu-id="4ad2e-123">Count of devices already CoManaged</span></span>|
|<span data-ttu-id="4ad2e-124">eligibleCount</span><span class="sxs-lookup"><span data-stu-id="4ad2e-124">eligibleCount</span></span>|<span data-ttu-id="4ad2e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="4ad2e-125">Int32</span></span>|<span data-ttu-id="4ad2e-126">Contagem de dispositivos totalmente qualificados para o cogerenciamento</span><span class="sxs-lookup"><span data-stu-id="4ad2e-126">Count of devices fully eligible for CoManagement</span></span>|
|<span data-ttu-id="4ad2e-127">eligibleButNotAadJoinedCount</span><span class="sxs-lookup"><span data-stu-id="4ad2e-127">eligibleButNotAadJoinedCount</span></span>|<span data-ttu-id="4ad2e-128">Int32</span><span class="sxs-lookup"><span data-stu-id="4ad2e-128">Int32</span></span>|<span data-ttu-id="4ad2e-129">Contagem de dispositivos qualificados para o cogerenciamento, mas ainda não ingressou no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="4ad2e-129">Count of devices eligible for CoManagement but not yet joined to Azure Active Directory</span></span>|
|<span data-ttu-id="4ad2e-130">needsOSUpdateCount</span><span class="sxs-lookup"><span data-stu-id="4ad2e-130">needsOSUpdateCount</span></span>|<span data-ttu-id="4ad2e-131">Int32</span><span class="sxs-lookup"><span data-stu-id="4ad2e-131">Int32</span></span>|<span data-ttu-id="4ad2e-132">Contagem de dispositivos que serão qualificados para cogerenciamento após uma atualização de so</span><span class="sxs-lookup"><span data-stu-id="4ad2e-132">Count of devices that will be eligible for CoManagement after an OS update</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ad2e-133">Relações</span><span class="sxs-lookup"><span data-stu-id="4ad2e-133">Relationships</span></span>
<span data-ttu-id="4ad2e-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ad2e-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ad2e-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ad2e-135">JSON Representation</span></span>
<span data-ttu-id="4ad2e-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.comanagementEligibleSummaryEntity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleSummaryEntity",
  "id": "String (identifier)",
  "coManagedCount": 1024,
  "eligibleCount": 1024,
  "eligibleButNotAadJoinedCount": 1024,
  "needsOSUpdateCount": 1024
}
```


---
title: tipo de recurso configurationManagerCollectionAssignmentTarget
description: Representa uma atribuição a uma coleção configuration manager.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cb43c23a0eafaefea0b9265102880de58008f153
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610869"
---
# <a name="configurationmanagercollectionassignmenttarget-resource-type"></a><span data-ttu-id="900ae-103">tipo de recurso configurationManagerCollectionAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="900ae-103">configurationManagerCollectionAssignmentTarget resource type</span></span>

<span data-ttu-id="900ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="900ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="900ae-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="900ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="900ae-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="900ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="900ae-107">Representa uma atribuição a uma coleção configuration manager.</span><span class="sxs-lookup"><span data-stu-id="900ae-107">Represents an assignment to a Configuration Manager Collection.</span></span>


<span data-ttu-id="900ae-108">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="900ae-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="900ae-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="900ae-109">Properties</span></span>
|<span data-ttu-id="900ae-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="900ae-110">Property</span></span>|<span data-ttu-id="900ae-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="900ae-111">Type</span></span>|<span data-ttu-id="900ae-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="900ae-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="900ae-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="900ae-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="900ae-114">String</span><span class="sxs-lookup"><span data-stu-id="900ae-114">String</span></span>|<span data-ttu-id="900ae-115">A ID do filtro para a atribuição de destino.</span><span class="sxs-lookup"><span data-stu-id="900ae-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="900ae-116">Herdado [de deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="900ae-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="900ae-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="900ae-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="900ae-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="900ae-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-devices-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="900ae-119">O tipo de filtro da atribuição de destino ou seja, Excluir ou Incluir.</span><span class="sxs-lookup"><span data-stu-id="900ae-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="900ae-120">Herdado [de deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="900ae-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="900ae-121">Os valores possíveis são: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="900ae-121">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="900ae-122">collectionId</span><span class="sxs-lookup"><span data-stu-id="900ae-122">collectionId</span></span>|<span data-ttu-id="900ae-123">String</span><span class="sxs-lookup"><span data-stu-id="900ae-123">String</span></span>|<span data-ttu-id="900ae-124">A ID da coleção que é o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="900ae-124">The collection Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="900ae-125">Relações</span><span class="sxs-lookup"><span data-stu-id="900ae-125">Relationships</span></span>
<span data-ttu-id="900ae-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="900ae-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="900ae-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="900ae-127">JSON Representation</span></span>
<span data-ttu-id="900ae-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="900ae-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerCollectionAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String",
  "collectionId": "String"
}
```





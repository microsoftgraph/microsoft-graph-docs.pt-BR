---
title: Tipo de recurso configurationManagerCollectionAssignmentTarget
description: Representa uma atribuição a uma coleção do Configuration Manager.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d32813e7c5c7cdae889406d694f686630311166
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160301"
---
# <a name="configurationmanagercollectionassignmenttarget-resource-type"></a><span data-ttu-id="45971-103">Tipo de recurso configurationManagerCollectionAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="45971-103">configurationManagerCollectionAssignmentTarget resource type</span></span>

<span data-ttu-id="45971-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45971-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45971-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45971-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45971-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45971-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45971-107">Representa uma atribuição a uma coleção do Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="45971-107">Represents an assignment to a Configuration Manager Collection.</span></span>


<span data-ttu-id="45971-108">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="45971-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="45971-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45971-109">Properties</span></span>
|<span data-ttu-id="45971-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45971-110">Property</span></span>|<span data-ttu-id="45971-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="45971-111">Type</span></span>|<span data-ttu-id="45971-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="45971-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45971-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="45971-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="45971-114">String</span><span class="sxs-lookup"><span data-stu-id="45971-114">String</span></span>|<span data-ttu-id="45971-115">A ID do filtro para a atribuição de destino.</span><span class="sxs-lookup"><span data-stu-id="45971-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="45971-116">Herdado [de deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="45971-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="45971-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="45971-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="45971-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="45971-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="45971-119">O tipo de filtro da atribuição de destino, ou seja, Excluir ou Incluir.</span><span class="sxs-lookup"><span data-stu-id="45971-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="45971-120">Herdado [de deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="45971-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="45971-121">Os valores possíveis são: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="45971-121">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="45971-122">collectionId</span><span class="sxs-lookup"><span data-stu-id="45971-122">collectionId</span></span>|<span data-ttu-id="45971-123">String</span><span class="sxs-lookup"><span data-stu-id="45971-123">String</span></span>|<span data-ttu-id="45971-124">A ID da coleção que é o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="45971-124">The collection Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45971-125">Relações</span><span class="sxs-lookup"><span data-stu-id="45971-125">Relationships</span></span>
<span data-ttu-id="45971-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="45971-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45971-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45971-127">JSON Representation</span></span>
<span data-ttu-id="45971-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="45971-128">Here is a JSON representation of the resource.</span></span>
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





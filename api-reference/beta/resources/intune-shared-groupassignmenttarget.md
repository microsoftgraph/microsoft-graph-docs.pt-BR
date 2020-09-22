---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8ede502c06ffcaef4f3d9be2f133ea6eb591d5de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084279"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="ac059-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ac059-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="ac059-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac059-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac059-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ac059-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac059-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ac059-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac059-107">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="ac059-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="ac059-108">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="ac059-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ac059-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac059-109">Properties</span></span>
|<span data-ttu-id="ac059-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac059-110">Property</span></span>|<span data-ttu-id="ac059-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac059-111">Type</span></span>|<span data-ttu-id="ac059-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac059-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac059-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="ac059-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="ac059-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac059-114">String</span></span>|<span data-ttu-id="ac059-115">A ID do filtro para a atribuição de destino.</span><span class="sxs-lookup"><span data-stu-id="ac059-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="ac059-116">Herdado de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="ac059-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="ac059-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="ac059-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="ac059-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="ac059-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="ac059-119">O tipo de filtro da atribuição de destino, ou seja, excluir ou incluir.</span><span class="sxs-lookup"><span data-stu-id="ac059-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="ac059-120">Herdado de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="ac059-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="ac059-121">Os valores possíveis são: `none` e `include`.</span><span class="sxs-lookup"><span data-stu-id="ac059-121">Possible values are: `none`, `include`.</span></span>|
|<span data-ttu-id="ac059-122">groupId</span><span class="sxs-lookup"><span data-stu-id="ac059-122">groupId</span></span>|<span data-ttu-id="ac059-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac059-123">String</span></span>|<span data-ttu-id="ac059-124">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="ac059-124">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac059-125">Relações</span><span class="sxs-lookup"><span data-stu-id="ac059-125">Relationships</span></span>
<span data-ttu-id="ac059-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac059-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac059-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac059-127">JSON Representation</span></span>
<span data-ttu-id="ac059-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac059-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String",
  "groupId": "String"
}
```







---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5800977f704b82ba83d82b7a0acdda8a2d6e6df2
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793427"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="2b69f-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2b69f-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="2b69f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b69f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b69f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2b69f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b69f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b69f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b69f-107">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="2b69f-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="2b69f-108">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="2b69f-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2b69f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b69f-109">Properties</span></span>
|<span data-ttu-id="2b69f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b69f-110">Property</span></span>|<span data-ttu-id="2b69f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b69f-111">Type</span></span>|<span data-ttu-id="2b69f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b69f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b69f-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="2b69f-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="2b69f-114">String</span><span class="sxs-lookup"><span data-stu-id="2b69f-114">String</span></span>|<span data-ttu-id="2b69f-115">A ID do filtro para a atribuição de destino.</span><span class="sxs-lookup"><span data-stu-id="2b69f-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="2b69f-116">Herdado de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="2b69f-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="2b69f-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="2b69f-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="2b69f-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="2b69f-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="2b69f-119">O tipo de filtro da atribuição de destino, ou seja, excluir ou incluir.</span><span class="sxs-lookup"><span data-stu-id="2b69f-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="2b69f-120">Herdado de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="2b69f-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="2b69f-121">Os valores possíveis são: `none` e `include`.</span><span class="sxs-lookup"><span data-stu-id="2b69f-121">Possible values are: `none`, `include`.</span></span>|
|<span data-ttu-id="2b69f-122">groupId</span><span class="sxs-lookup"><span data-stu-id="2b69f-122">groupId</span></span>|<span data-ttu-id="2b69f-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b69f-123">String</span></span>|<span data-ttu-id="2b69f-124">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="2b69f-124">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b69f-125">Relações</span><span class="sxs-lookup"><span data-stu-id="2b69f-125">Relationships</span></span>
<span data-ttu-id="2b69f-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2b69f-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b69f-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b69f-127">JSON Representation</span></span>
<span data-ttu-id="2b69f-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b69f-128">Here is a JSON representation of the resource.</span></span>
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




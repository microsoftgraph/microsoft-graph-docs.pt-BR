---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 70b53e52db8a2dba6f5c8b426e684957b2271d62
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735117"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="2cafa-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2cafa-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="2cafa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cafa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2cafa-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2cafa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cafa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2cafa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cafa-107">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="2cafa-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="2cafa-108">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="2cafa-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2cafa-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2cafa-109">Properties</span></span>
|<span data-ttu-id="2cafa-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2cafa-110">Property</span></span>|<span data-ttu-id="2cafa-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cafa-111">Type</span></span>|<span data-ttu-id="2cafa-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cafa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cafa-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="2cafa-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="2cafa-114">String</span><span class="sxs-lookup"><span data-stu-id="2cafa-114">String</span></span>|<span data-ttu-id="2cafa-115">A ID do filtro para a atribuição de destino.</span><span class="sxs-lookup"><span data-stu-id="2cafa-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="2cafa-116">Herdado de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="2cafa-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="2cafa-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="2cafa-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="2cafa-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="2cafa-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="2cafa-119">O tipo de filtro da atribuição de destino, ou seja, excluir ou incluir.</span><span class="sxs-lookup"><span data-stu-id="2cafa-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="2cafa-120">Herdado de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="2cafa-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="2cafa-121">Os valores possíveis são: `none` e `include`.</span><span class="sxs-lookup"><span data-stu-id="2cafa-121">Possible values are: `none`, `include`.</span></span>|
|<span data-ttu-id="2cafa-122">groupId</span><span class="sxs-lookup"><span data-stu-id="2cafa-122">groupId</span></span>|<span data-ttu-id="2cafa-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2cafa-123">String</span></span>|<span data-ttu-id="2cafa-124">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="2cafa-124">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cafa-125">Relações</span><span class="sxs-lookup"><span data-stu-id="2cafa-125">Relationships</span></span>
<span data-ttu-id="2cafa-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2cafa-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cafa-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2cafa-127">JSON Representation</span></span>
<span data-ttu-id="2cafa-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2cafa-128">Here is a JSON representation of the resource.</span></span>
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






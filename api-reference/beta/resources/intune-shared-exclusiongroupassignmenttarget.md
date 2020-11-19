---
title: Tipo de recurso exclusionGroupAssignmentTarget
description: Representa um grupo que deve ser excluído de uma atribuição.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a8b9b8d861bdeb0091bec28381c2a84eec04889a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49258966"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="d5dba-103">Tipo de recurso exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d5dba-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="d5dba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5dba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5dba-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d5dba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5dba-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5dba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5dba-107">Representa um grupo que deve ser excluído de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="d5dba-107">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="d5dba-108">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="d5dba-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d5dba-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5dba-109">Properties</span></span>
|<span data-ttu-id="d5dba-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5dba-110">Property</span></span>|<span data-ttu-id="d5dba-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5dba-111">Type</span></span>|<span data-ttu-id="d5dba-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5dba-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5dba-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="d5dba-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="d5dba-114">String</span><span class="sxs-lookup"><span data-stu-id="d5dba-114">String</span></span>|<span data-ttu-id="d5dba-115">A ID do filtro para a atribuição de destino.</span><span class="sxs-lookup"><span data-stu-id="d5dba-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="d5dba-116">Herdado de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="d5dba-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="d5dba-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="d5dba-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="d5dba-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="d5dba-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="d5dba-119">O tipo de filtro da atribuição de destino, ou seja, excluir ou incluir.</span><span class="sxs-lookup"><span data-stu-id="d5dba-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="d5dba-120">Herdado de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="d5dba-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="d5dba-121">Os valores possíveis são: `none` e `include`.</span><span class="sxs-lookup"><span data-stu-id="d5dba-121">Possible values are: `none`, `include`.</span></span>|
|<span data-ttu-id="d5dba-122">groupId</span><span class="sxs-lookup"><span data-stu-id="d5dba-122">groupId</span></span>|<span data-ttu-id="d5dba-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5dba-123">String</span></span>|<span data-ttu-id="d5dba-124">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="d5dba-124">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="d5dba-125">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="d5dba-125">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5dba-126">Relações</span><span class="sxs-lookup"><span data-stu-id="d5dba-126">Relationships</span></span>
<span data-ttu-id="d5dba-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5dba-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5dba-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5dba-128">JSON Representation</span></span>
<span data-ttu-id="d5dba-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5dba-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String",
  "groupId": "String"
}
```





---
title: Tipo de recurso allLicensedUsersAssignmentTarget
description: Representa uma atribuição para todos os usuários licenciados no locatário.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4388710e079366193f2a2ca7bd842a2d7b5763cf
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793595"
---
# <a name="alllicensedusersassignmenttarget-resource-type"></a><span data-ttu-id="0ef7a-103">Tipo de recurso allLicensedUsersAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0ef7a-103">allLicensedUsersAssignmentTarget resource type</span></span>

<span data-ttu-id="0ef7a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ef7a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ef7a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0ef7a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ef7a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ef7a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ef7a-107">Representa uma atribuição para todos os usuários licenciados no locatário.</span><span class="sxs-lookup"><span data-stu-id="0ef7a-107">Represents an assignment to all licensed users in the tenant.</span></span>


<span data-ttu-id="0ef7a-108">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="0ef7a-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0ef7a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ef7a-109">Properties</span></span>
|<span data-ttu-id="0ef7a-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ef7a-110">Property</span></span>|<span data-ttu-id="0ef7a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ef7a-111">Type</span></span>|<span data-ttu-id="0ef7a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ef7a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ef7a-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="0ef7a-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="0ef7a-114">String</span><span class="sxs-lookup"><span data-stu-id="0ef7a-114">String</span></span>|<span data-ttu-id="0ef7a-115">A ID do filtro para a atribuição de destino.</span><span class="sxs-lookup"><span data-stu-id="0ef7a-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="0ef7a-116">Herdado de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="0ef7a-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="0ef7a-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="0ef7a-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="0ef7a-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="0ef7a-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="0ef7a-119">O tipo de filtro da atribuição de destino, ou seja, excluir ou incluir.</span><span class="sxs-lookup"><span data-stu-id="0ef7a-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="0ef7a-120">Herdado de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="0ef7a-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="0ef7a-121">Os valores possíveis são: `none`, `include`.</span><span class="sxs-lookup"><span data-stu-id="0ef7a-121">Possible values are: `none`, `include`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ef7a-122">Relações</span><span class="sxs-lookup"><span data-stu-id="0ef7a-122">Relationships</span></span>
<span data-ttu-id="0ef7a-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0ef7a-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ef7a-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ef7a-124">JSON Representation</span></span>
<span data-ttu-id="0ef7a-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ef7a-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.allLicensedUsersAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String"
}
```




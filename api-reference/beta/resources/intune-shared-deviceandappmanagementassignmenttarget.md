---
title: Tipo de recurso deviceAndAppManagementAssignmentTarget
description: Tipo base para destinos de atribuição.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4194d5afb7f7c90f658c558d8609badef2d89cfc
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793490"
---
# <a name="deviceandappmanagementassignmenttarget-resource-type"></a><span data-ttu-id="2fb58-103">Tipo de recurso deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2fb58-103">deviceAndAppManagementAssignmentTarget resource type</span></span>

<span data-ttu-id="2fb58-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fb58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2fb58-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2fb58-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fb58-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2fb58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fb58-107">Tipo base para destinos de atribuição.</span><span class="sxs-lookup"><span data-stu-id="2fb58-107">Base type for assignment targets.</span></span>

## <a name="properties"></a><span data-ttu-id="2fb58-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2fb58-108">Properties</span></span>
|<span data-ttu-id="2fb58-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fb58-109">Property</span></span>|<span data-ttu-id="2fb58-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fb58-110">Type</span></span>|<span data-ttu-id="2fb58-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fb58-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fb58-112">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="2fb58-112">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="2fb58-113">String</span><span class="sxs-lookup"><span data-stu-id="2fb58-113">String</span></span>|<span data-ttu-id="2fb58-114">A ID do filtro para a atribuição de destino.</span><span class="sxs-lookup"><span data-stu-id="2fb58-114">The Id of the filter for the target assignment.</span></span>|
|<span data-ttu-id="2fb58-115">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="2fb58-115">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="2fb58-116">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="2fb58-116">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="2fb58-117">O tipo de filtro da atribuição de destino, ou seja, excluir ou incluir.</span><span class="sxs-lookup"><span data-stu-id="2fb58-117">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="2fb58-118">Os valores possíveis são: `none`, `include`.</span><span class="sxs-lookup"><span data-stu-id="2fb58-118">Possible values are: `none`, `include`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fb58-119">Relações</span><span class="sxs-lookup"><span data-stu-id="2fb58-119">Relationships</span></span>
<span data-ttu-id="2fb58-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2fb58-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fb58-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2fb58-121">JSON Representation</span></span>
<span data-ttu-id="2fb58-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2fb58-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String"
}
```




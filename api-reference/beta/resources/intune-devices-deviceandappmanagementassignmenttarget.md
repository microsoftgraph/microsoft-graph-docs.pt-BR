---
title: Tipo de recurso deviceAndAppManagementAssignmentTarget
description: Tipo base para destinos de atribuição.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7bc5618c45e5e0a1c7320e5e8196cd6429b484cb
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611773"
---
# <a name="deviceandappmanagementassignmenttarget-resource-type"></a><span data-ttu-id="ceee7-103">Tipo de recurso deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ceee7-103">deviceAndAppManagementAssignmentTarget resource type</span></span>

<span data-ttu-id="ceee7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ceee7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ceee7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ceee7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ceee7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ceee7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ceee7-107">Tipo base para destinos de atribuição.</span><span class="sxs-lookup"><span data-stu-id="ceee7-107">Base type for assignment targets.</span></span>

## <a name="properties"></a><span data-ttu-id="ceee7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ceee7-108">Properties</span></span>
|<span data-ttu-id="ceee7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ceee7-109">Property</span></span>|<span data-ttu-id="ceee7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ceee7-110">Type</span></span>|<span data-ttu-id="ceee7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ceee7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ceee7-112">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="ceee7-112">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="ceee7-113">String</span><span class="sxs-lookup"><span data-stu-id="ceee7-113">String</span></span>|<span data-ttu-id="ceee7-114">A ID do filtro para a atribuição de destino.</span><span class="sxs-lookup"><span data-stu-id="ceee7-114">The Id of the filter for the target assignment.</span></span>|
|<span data-ttu-id="ceee7-115">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="ceee7-115">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="ceee7-116">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="ceee7-116">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-devices-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="ceee7-117">O tipo de filtro da atribuição de destino ou seja, Excluir ou Incluir.</span><span class="sxs-lookup"><span data-stu-id="ceee7-117">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="ceee7-118">Os valores possíveis são: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="ceee7-118">Possible values are: `none`, `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ceee7-119">Relações</span><span class="sxs-lookup"><span data-stu-id="ceee7-119">Relationships</span></span>
<span data-ttu-id="ceee7-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ceee7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ceee7-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ceee7-121">JSON Representation</span></span>
<span data-ttu-id="ceee7-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ceee7-122">Here is a JSON representation of the resource.</span></span>
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





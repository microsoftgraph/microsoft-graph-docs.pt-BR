---
title: Tipo de recurso deviceAndAppManagementAssignmentTarget
description: Tipo base para destinos de atribuição.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2534552af331a3a41ce45fcc97a74717c666b019
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49266197"
---
# <a name="deviceandappmanagementassignmenttarget-resource-type"></a><span data-ttu-id="04e4d-103">Tipo de recurso deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="04e4d-103">deviceAndAppManagementAssignmentTarget resource type</span></span>

<span data-ttu-id="04e4d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04e4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04e4d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04e4d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04e4d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04e4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04e4d-107">Tipo base para destinos de atribuição.</span><span class="sxs-lookup"><span data-stu-id="04e4d-107">Base type for assignment targets.</span></span>

## <a name="properties"></a><span data-ttu-id="04e4d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04e4d-108">Properties</span></span>
|<span data-ttu-id="04e4d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04e4d-109">Property</span></span>|<span data-ttu-id="04e4d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="04e4d-110">Type</span></span>|<span data-ttu-id="04e4d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="04e4d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04e4d-112">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="04e4d-112">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="04e4d-113">String</span><span class="sxs-lookup"><span data-stu-id="04e4d-113">String</span></span>|<span data-ttu-id="04e4d-114">A ID do filtro para a atribuição de destino.</span><span class="sxs-lookup"><span data-stu-id="04e4d-114">The Id of the filter for the target assignment.</span></span>|
|<span data-ttu-id="04e4d-115">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="04e4d-115">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="04e4d-116">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="04e4d-116">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="04e4d-117">O tipo de filtro da atribuição de destino, ou seja, excluir ou incluir.</span><span class="sxs-lookup"><span data-stu-id="04e4d-117">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="04e4d-118">Os valores possíveis são: `none`, `include`.</span><span class="sxs-lookup"><span data-stu-id="04e4d-118">Possible values are: `none`, `include`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04e4d-119">Relações</span><span class="sxs-lookup"><span data-stu-id="04e4d-119">Relationships</span></span>
<span data-ttu-id="04e4d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04e4d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04e4d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04e4d-121">JSON Representation</span></span>
<span data-ttu-id="04e4d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04e4d-122">Here is a JSON representation of the resource.</span></span>
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





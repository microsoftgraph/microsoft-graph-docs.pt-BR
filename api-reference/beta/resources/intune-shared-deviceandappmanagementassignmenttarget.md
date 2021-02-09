---
title: Tipo de recurso deviceAndAppManagementAssignmentTarget
description: Tipo base para destinos de atribuição.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ec96f18f16a40182bccfc00efbe70c84568fae33
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158090"
---
# <a name="deviceandappmanagementassignmenttarget-resource-type"></a><span data-ttu-id="87290-103">Tipo de recurso deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="87290-103">deviceAndAppManagementAssignmentTarget resource type</span></span>

<span data-ttu-id="87290-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87290-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87290-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="87290-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87290-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87290-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87290-107">Tipo base para destinos de atribuição.</span><span class="sxs-lookup"><span data-stu-id="87290-107">Base type for assignment targets.</span></span>

## <a name="properties"></a><span data-ttu-id="87290-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87290-108">Properties</span></span>
|<span data-ttu-id="87290-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87290-109">Property</span></span>|<span data-ttu-id="87290-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="87290-110">Type</span></span>|<span data-ttu-id="87290-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="87290-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87290-112">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="87290-112">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="87290-113">String</span><span class="sxs-lookup"><span data-stu-id="87290-113">String</span></span>|<span data-ttu-id="87290-114">A ID do filtro para a atribuição de destino.</span><span class="sxs-lookup"><span data-stu-id="87290-114">The Id of the filter for the target assignment.</span></span>|
|<span data-ttu-id="87290-115">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="87290-115">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="87290-116">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="87290-116">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="87290-117">O tipo de filtro da atribuição de destino, ou seja, Excluir ou Incluir.</span><span class="sxs-lookup"><span data-stu-id="87290-117">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="87290-118">Os valores possíveis são: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="87290-118">Possible values are: `none`, `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87290-119">Relações</span><span class="sxs-lookup"><span data-stu-id="87290-119">Relationships</span></span>
<span data-ttu-id="87290-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="87290-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87290-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87290-121">JSON Representation</span></span>
<span data-ttu-id="87290-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87290-122">Here is a JSON representation of the resource.</span></span>
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





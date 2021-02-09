---
title: Tipo de recurso allLicensedUsersAssignmentTarget
description: Representa uma atribuição para todos os usuários licenciados no locatário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1f4e05236b0782d74547204bab30d7957aeb52ca
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158412"
---
# <a name="alllicensedusersassignmenttarget-resource-type"></a><span data-ttu-id="64eeb-103">Tipo de recurso allLicensedUsersAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="64eeb-103">allLicensedUsersAssignmentTarget resource type</span></span>

<span data-ttu-id="64eeb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64eeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64eeb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64eeb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64eeb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64eeb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64eeb-107">Representa uma atribuição para todos os usuários licenciados no locatário.</span><span class="sxs-lookup"><span data-stu-id="64eeb-107">Represents an assignment to all licensed users in the tenant.</span></span>


<span data-ttu-id="64eeb-108">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="64eeb-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="64eeb-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64eeb-109">Properties</span></span>
|<span data-ttu-id="64eeb-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64eeb-110">Property</span></span>|<span data-ttu-id="64eeb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="64eeb-111">Type</span></span>|<span data-ttu-id="64eeb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="64eeb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64eeb-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="64eeb-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="64eeb-114">String</span><span class="sxs-lookup"><span data-stu-id="64eeb-114">String</span></span>|<span data-ttu-id="64eeb-115">A ID do filtro para a atribuição de destino.</span><span class="sxs-lookup"><span data-stu-id="64eeb-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="64eeb-116">Herdado [de deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="64eeb-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="64eeb-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="64eeb-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="64eeb-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="64eeb-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="64eeb-119">O tipo de filtro da atribuição de destino, ou seja, Excluir ou Incluir.</span><span class="sxs-lookup"><span data-stu-id="64eeb-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="64eeb-120">Herdado [de deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="64eeb-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="64eeb-121">Os valores possíveis são: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="64eeb-121">Possible values are: `none`, `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64eeb-122">Relações</span><span class="sxs-lookup"><span data-stu-id="64eeb-122">Relationships</span></span>
<span data-ttu-id="64eeb-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64eeb-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64eeb-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64eeb-124">JSON Representation</span></span>
<span data-ttu-id="64eeb-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64eeb-125">Here is a JSON representation of the resource.</span></span>
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





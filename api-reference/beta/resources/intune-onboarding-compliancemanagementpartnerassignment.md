---
title: tipo de recurso complianceManagementPartnerAssignment
description: Direcionamento de grupo de usuários para parceiro de gerenciamento de conformidade
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6b557cde710ac0d2a4820c71b7e595ad49e6f026
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697305"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="f346a-103">tipo de recurso complianceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="f346a-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="f346a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f346a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f346a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f346a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f346a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f346a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f346a-107">Direcionamento de grupo de usuários para parceiro de gerenciamento de conformidade</span><span class="sxs-lookup"><span data-stu-id="f346a-107">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="f346a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f346a-108">Properties</span></span>
|<span data-ttu-id="f346a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f346a-109">Property</span></span>|<span data-ttu-id="f346a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f346a-110">Type</span></span>|<span data-ttu-id="f346a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f346a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f346a-112">destino</span><span class="sxs-lookup"><span data-stu-id="f346a-112">target</span></span>|[<span data-ttu-id="f346a-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f346a-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f346a-114">Destino de atribuição de grupo.</span><span class="sxs-lookup"><span data-stu-id="f346a-114">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f346a-115">Relações</span><span class="sxs-lookup"><span data-stu-id="f346a-115">Relationships</span></span>
<span data-ttu-id="f346a-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f346a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f346a-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f346a-117">JSON Representation</span></span>
<span data-ttu-id="f346a-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f346a-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```






---
title: tipo de recurso complianceManagementPartnerAssignment
description: Direcionamento de grupo de usuários para parceiro de gerenciamento de conformidade
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed6a9b6fe9c1262dcc54b851f84a40096b2cb04c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222741"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="7b94d-103">tipo de recurso complianceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="7b94d-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="7b94d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b94d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b94d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7b94d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b94d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7b94d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b94d-107">Direcionamento de grupo de usuários para parceiro de gerenciamento de conformidade</span><span class="sxs-lookup"><span data-stu-id="7b94d-107">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="7b94d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b94d-108">Properties</span></span>
|<span data-ttu-id="7b94d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b94d-109">Property</span></span>|<span data-ttu-id="7b94d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b94d-110">Type</span></span>|<span data-ttu-id="7b94d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b94d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b94d-112">destino</span><span class="sxs-lookup"><span data-stu-id="7b94d-112">target</span></span>|[<span data-ttu-id="7b94d-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7b94d-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7b94d-114">Destino de atribuição de grupo.</span><span class="sxs-lookup"><span data-stu-id="7b94d-114">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b94d-115">Relações</span><span class="sxs-lookup"><span data-stu-id="7b94d-115">Relationships</span></span>
<span data-ttu-id="7b94d-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b94d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b94d-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b94d-117">JSON Representation</span></span>
<span data-ttu-id="7b94d-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b94d-118">Here is a JSON representation of the resource.</span></span>
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





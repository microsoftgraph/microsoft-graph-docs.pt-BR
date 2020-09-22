---
title: tipo de recurso complianceManagementPartnerAssignment
description: Direcionamento de grupo de usuários para parceiro de gerenciamento de conformidade
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d9bdcfd0edcdf4e93b3bf11f8d30a3cef5cc9d60
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072967"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="82ff8-103">tipo de recurso complianceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="82ff8-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="82ff8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82ff8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82ff8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82ff8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82ff8-106">Direcionamento de grupo de usuários para parceiro de gerenciamento de conformidade</span><span class="sxs-lookup"><span data-stu-id="82ff8-106">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="82ff8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82ff8-107">Properties</span></span>
|<span data-ttu-id="82ff8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82ff8-108">Property</span></span>|<span data-ttu-id="82ff8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="82ff8-109">Type</span></span>|<span data-ttu-id="82ff8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="82ff8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82ff8-111">destino</span><span class="sxs-lookup"><span data-stu-id="82ff8-111">target</span></span>|[<span data-ttu-id="82ff8-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="82ff8-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="82ff8-113">Destino de atribuição de grupo.</span><span class="sxs-lookup"><span data-stu-id="82ff8-113">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82ff8-114">Relações</span><span class="sxs-lookup"><span data-stu-id="82ff8-114">Relationships</span></span>
<span data-ttu-id="82ff8-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="82ff8-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82ff8-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82ff8-116">JSON Representation</span></span>
<span data-ttu-id="82ff8-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="82ff8-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```






---
title: tipo de recurso complianceManagementPartnerAssignment
description: Direcionamento de grupo de usuários para parceiro de gerenciamento de conformidade
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6cf246cd1f7fad0d168165f72a3861005e8cefbe
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744103"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="a4950-103">tipo de recurso complianceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="a4950-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="a4950-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4950-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4950-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a4950-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4950-106">Direcionamento de grupo de usuários para parceiro de gerenciamento de conformidade</span><span class="sxs-lookup"><span data-stu-id="a4950-106">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="a4950-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4950-107">Properties</span></span>
|<span data-ttu-id="a4950-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4950-108">Property</span></span>|<span data-ttu-id="a4950-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4950-109">Type</span></span>|<span data-ttu-id="a4950-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4950-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4950-111">destino</span><span class="sxs-lookup"><span data-stu-id="a4950-111">target</span></span>|[<span data-ttu-id="a4950-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a4950-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a4950-113">Destino de atribuição de grupo.</span><span class="sxs-lookup"><span data-stu-id="a4950-113">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4950-114">Relações</span><span class="sxs-lookup"><span data-stu-id="a4950-114">Relationships</span></span>
<span data-ttu-id="a4950-115">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a4950-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4950-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4950-116">JSON Representation</span></span>
<span data-ttu-id="a4950-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a4950-117">Here is a JSON representation of the resource.</span></span>
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




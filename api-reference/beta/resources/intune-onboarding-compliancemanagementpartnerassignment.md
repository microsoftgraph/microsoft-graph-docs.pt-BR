---
title: tipo de recurso complianceManagementPartnerAssignment
description: Direcionamento de grupo de usuários para parceiro de gerenciamento de conformidade
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 51dc2a8f4861f160db6a3775526ec7fdd4e85ea7
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088214"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="a3b9a-103">tipo de recurso complianceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="a3b9a-103">complianceManagementPartnerAssignment resource type</span></span>

> <span data-ttu-id="a3b9a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a3b9a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3b9a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a3b9a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3b9a-106">Direcionamento de grupo de usuários para parceiro de gerenciamento de conformidade</span><span class="sxs-lookup"><span data-stu-id="a3b9a-106">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="a3b9a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3b9a-107">Properties</span></span>
|<span data-ttu-id="a3b9a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3b9a-108">Property</span></span>|<span data-ttu-id="a3b9a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3b9a-109">Type</span></span>|<span data-ttu-id="a3b9a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3b9a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3b9a-111">destino</span><span class="sxs-lookup"><span data-stu-id="a3b9a-111">target</span></span>|[<span data-ttu-id="a3b9a-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a3b9a-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a3b9a-113">Destino de atribuição de grupo.</span><span class="sxs-lookup"><span data-stu-id="a3b9a-113">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3b9a-114">Relações</span><span class="sxs-lookup"><span data-stu-id="a3b9a-114">Relationships</span></span>
<span data-ttu-id="a3b9a-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a3b9a-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3b9a-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3b9a-116">JSON Representation</span></span>
<span data-ttu-id="a3b9a-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a3b9a-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




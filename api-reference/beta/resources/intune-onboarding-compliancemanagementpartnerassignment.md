---
title: tipo de recurso complianceManagementPartnerAssignment
description: Direcionamento de grupo de usuários para parceiro de gerenciamento de conformidade
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 833a2dee09caae20b9a58fb5c82d9de06ce5cf33
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43418956"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="9a4ad-103">tipo de recurso complianceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="9a4ad-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="9a4ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a4ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a4ad-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a4ad-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a4ad-107">Direcionamento de grupo de usuários para parceiro de gerenciamento de conformidade</span><span class="sxs-lookup"><span data-stu-id="9a4ad-107">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="9a4ad-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a4ad-108">Properties</span></span>
|<span data-ttu-id="9a4ad-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a4ad-109">Property</span></span>|<span data-ttu-id="9a4ad-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a4ad-110">Type</span></span>|<span data-ttu-id="9a4ad-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a4ad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a4ad-112">destino</span><span class="sxs-lookup"><span data-stu-id="9a4ad-112">target</span></span>|[<span data-ttu-id="9a4ad-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9a4ad-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9a4ad-114">Destino de atribuição de grupo.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-114">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a4ad-115">Relações</span><span class="sxs-lookup"><span data-stu-id="9a4ad-115">Relationships</span></span>
<span data-ttu-id="9a4ad-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9a4ad-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a4ad-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a4ad-117">JSON Representation</span></span>
<span data-ttu-id="9a4ad-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-118">Here is a JSON representation of the resource.</span></span>
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




---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 62de6a0a085fda974d9f8140aa2961e6a3610cb4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967424"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="cce13-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cce13-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="cce13-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cce13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cce13-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cce13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cce13-106">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="cce13-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="cce13-107">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="cce13-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cce13-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cce13-108">Properties</span></span>
|<span data-ttu-id="cce13-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cce13-109">Property</span></span>|<span data-ttu-id="cce13-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cce13-110">Type</span></span>|<span data-ttu-id="cce13-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cce13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cce13-112">groupId</span><span class="sxs-lookup"><span data-stu-id="cce13-112">groupId</span></span>|<span data-ttu-id="cce13-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cce13-113">String</span></span>|<span data-ttu-id="cce13-114">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="cce13-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cce13-115">Relações</span><span class="sxs-lookup"><span data-stu-id="cce13-115">Relationships</span></span>
<span data-ttu-id="cce13-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cce13-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cce13-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cce13-117">JSON Representation</span></span>
<span data-ttu-id="cce13-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cce13-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```






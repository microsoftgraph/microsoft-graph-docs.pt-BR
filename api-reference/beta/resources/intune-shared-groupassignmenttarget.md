---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3bb1de3dbd95145bc7f1ce631175e9867deb1dde
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43407691"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="7c15f-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7c15f-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="7c15f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c15f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c15f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7c15f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c15f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c15f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c15f-107">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="7c15f-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="7c15f-108">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="7c15f-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7c15f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c15f-109">Properties</span></span>
|<span data-ttu-id="7c15f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c15f-110">Property</span></span>|<span data-ttu-id="7c15f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c15f-111">Type</span></span>|<span data-ttu-id="7c15f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c15f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c15f-113">groupId</span><span class="sxs-lookup"><span data-stu-id="7c15f-113">groupId</span></span>|<span data-ttu-id="7c15f-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c15f-114">String</span></span>|<span data-ttu-id="7c15f-115">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="7c15f-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c15f-116">Relações</span><span class="sxs-lookup"><span data-stu-id="7c15f-116">Relationships</span></span>
<span data-ttu-id="7c15f-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7c15f-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c15f-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c15f-118">JSON Representation</span></span>
<span data-ttu-id="7c15f-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7c15f-119">Here is a JSON representation of the resource.</span></span>
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




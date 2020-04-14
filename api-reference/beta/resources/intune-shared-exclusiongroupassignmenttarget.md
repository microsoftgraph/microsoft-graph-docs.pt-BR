---
title: Tipo de recurso exclusionGroupAssignmentTarget
description: Representa um grupo que deve ser excluído de uma atribuição.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6c92cbad6b9c09de3dc8e468ddcec9d2035cb254
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43408049"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="3592b-103">Tipo de recurso exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3592b-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="3592b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3592b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3592b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3592b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3592b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3592b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3592b-107">Representa um grupo que deve ser excluído de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="3592b-107">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="3592b-108">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="3592b-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3592b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3592b-109">Properties</span></span>
|<span data-ttu-id="3592b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3592b-110">Property</span></span>|<span data-ttu-id="3592b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3592b-111">Type</span></span>|<span data-ttu-id="3592b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3592b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3592b-113">groupId</span><span class="sxs-lookup"><span data-stu-id="3592b-113">groupId</span></span>|<span data-ttu-id="3592b-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3592b-114">String</span></span>|<span data-ttu-id="3592b-115">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="3592b-115">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="3592b-116">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="3592b-116">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3592b-117">Relações</span><span class="sxs-lookup"><span data-stu-id="3592b-117">Relationships</span></span>
<span data-ttu-id="3592b-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3592b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3592b-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3592b-119">JSON Representation</span></span>
<span data-ttu-id="3592b-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3592b-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```




---
title: Tipo de recurso exclusionGroupAssignmentTarget
description: Representa um grupo que deve ser excluído de uma atribuição.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 805f2f1dbcab8751d564fbde3f6747b6e77f6d09
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036922"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="6f062-103">Tipo de recurso exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6f062-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="6f062-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f062-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f062-105">Representa um grupo que deve ser excluído de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="6f062-105">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="6f062-106">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="6f062-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6f062-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f062-107">Properties</span></span>
|<span data-ttu-id="6f062-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f062-108">Property</span></span>|<span data-ttu-id="6f062-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f062-109">Type</span></span>|<span data-ttu-id="6f062-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f062-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f062-111">groupId</span><span class="sxs-lookup"><span data-stu-id="6f062-111">groupId</span></span>|<span data-ttu-id="6f062-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f062-112">String</span></span>|<span data-ttu-id="6f062-113">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="6f062-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="6f062-114">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="6f062-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f062-115">Relações</span><span class="sxs-lookup"><span data-stu-id="6f062-115">Relationships</span></span>
<span data-ttu-id="6f062-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6f062-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f062-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f062-117">JSON Representation</span></span>
<span data-ttu-id="6f062-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f062-118">Here is a JSON representation of the resource.</span></span>
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




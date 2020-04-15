---
title: Tipo de recurso exclusionGroupAssignmentTarget
description: Representa um grupo que deve ser excluído de uma atribuição.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 535f6ed5e9dc81c3c39c4d0f56c7e5e38e79b5e5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445714"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="9c82f-103">Tipo de recurso exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9c82f-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="9c82f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c82f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c82f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c82f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c82f-106">Representa um grupo que deve ser excluído de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="9c82f-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="9c82f-107">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="9c82f-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9c82f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c82f-108">Properties</span></span>
|<span data-ttu-id="9c82f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c82f-109">Property</span></span>|<span data-ttu-id="9c82f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c82f-110">Type</span></span>|<span data-ttu-id="9c82f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c82f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c82f-112">groupId</span><span class="sxs-lookup"><span data-stu-id="9c82f-112">groupId</span></span>|<span data-ttu-id="9c82f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c82f-113">String</span></span>|<span data-ttu-id="9c82f-114">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="9c82f-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="9c82f-115">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="9c82f-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c82f-116">Relações</span><span class="sxs-lookup"><span data-stu-id="9c82f-116">Relationships</span></span>
<span data-ttu-id="9c82f-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c82f-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c82f-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c82f-118">JSON Representation</span></span>
<span data-ttu-id="9c82f-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c82f-119">Here is a JSON representation of the resource.</span></span>
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








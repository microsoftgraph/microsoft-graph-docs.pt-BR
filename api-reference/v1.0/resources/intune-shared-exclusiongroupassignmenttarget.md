---
title: Tipo de recurso exclusionGroupAssignmentTarget
description: Representa um grupo que deve ser excluído de uma atribuição.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3b0048cccfa9461bed2f1b25600b677512d45a47
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967510"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="62ba7-103">Tipo de recurso exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="62ba7-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="62ba7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62ba7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62ba7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62ba7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62ba7-106">Representa um grupo que deve ser excluído de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="62ba7-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="62ba7-107">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="62ba7-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="62ba7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62ba7-108">Properties</span></span>
|<span data-ttu-id="62ba7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62ba7-109">Property</span></span>|<span data-ttu-id="62ba7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="62ba7-110">Type</span></span>|<span data-ttu-id="62ba7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="62ba7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62ba7-112">groupId</span><span class="sxs-lookup"><span data-stu-id="62ba7-112">groupId</span></span>|<span data-ttu-id="62ba7-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62ba7-113">String</span></span>|<span data-ttu-id="62ba7-114">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="62ba7-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="62ba7-115">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="62ba7-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="62ba7-116">Relações</span><span class="sxs-lookup"><span data-stu-id="62ba7-116">Relationships</span></span>
<span data-ttu-id="62ba7-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="62ba7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62ba7-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62ba7-118">JSON Representation</span></span>
<span data-ttu-id="62ba7-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62ba7-119">Here is a JSON representation of the resource.</span></span>
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










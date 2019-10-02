---
title: Tipo de recurso exclusionGroupAssignmentTarget
description: Representa um grupo que deve ser excluído de uma atribuição.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 52dcbfe4337fdc5993f6f2b9499244f87a10b953
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354018"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="fbd97-103">Tipo de recurso exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fbd97-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="fbd97-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fbd97-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbd97-105">Representa um grupo que deve ser excluído de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="fbd97-105">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="fbd97-106">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="fbd97-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fbd97-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbd97-107">Properties</span></span>
|<span data-ttu-id="fbd97-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbd97-108">Property</span></span>|<span data-ttu-id="fbd97-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbd97-109">Type</span></span>|<span data-ttu-id="fbd97-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbd97-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbd97-111">groupId</span><span class="sxs-lookup"><span data-stu-id="fbd97-111">groupId</span></span>|<span data-ttu-id="fbd97-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbd97-112">String</span></span>|<span data-ttu-id="fbd97-113">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="fbd97-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="fbd97-114">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="fbd97-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbd97-115">Relações</span><span class="sxs-lookup"><span data-stu-id="fbd97-115">Relationships</span></span>
<span data-ttu-id="fbd97-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fbd97-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbd97-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbd97-117">JSON Representation</span></span>
<span data-ttu-id="fbd97-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fbd97-118">Here is a JSON representation of the resource.</span></span>
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





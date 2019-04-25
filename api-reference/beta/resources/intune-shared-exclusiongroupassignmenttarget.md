---
title: Tipo de recurso exclusionGroupAssignmentTarget
description: Representa um grupo que deve ser excluído de uma atribuição.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbd211bec428ff3a03ff989fa9ece36e5c55c561
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525247"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="bb46d-103">Tipo de recurso exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bb46d-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="bb46d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb46d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb46d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb46d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb46d-106">Representa um grupo que deve ser excluído de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="bb46d-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="bb46d-107">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="bb46d-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bb46d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb46d-108">Properties</span></span>
|<span data-ttu-id="bb46d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb46d-109">Property</span></span>|<span data-ttu-id="bb46d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb46d-110">Type</span></span>|<span data-ttu-id="bb46d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb46d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb46d-112">groupId</span><span class="sxs-lookup"><span data-stu-id="bb46d-112">groupId</span></span>|<span data-ttu-id="bb46d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb46d-113">String</span></span>|<span data-ttu-id="bb46d-114">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="bb46d-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="bb46d-115">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="bb46d-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb46d-116">Relações</span><span class="sxs-lookup"><span data-stu-id="bb46d-116">Relationships</span></span>
<span data-ttu-id="bb46d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb46d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb46d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb46d-118">JSON Representation</span></span>
<span data-ttu-id="bb46d-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb46d-119">Here is a JSON representation of the resource.</span></span>
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






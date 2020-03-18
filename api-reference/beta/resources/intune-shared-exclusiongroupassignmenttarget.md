---
title: Tipo de recurso exclusionGroupAssignmentTarget
description: Representa um grupo que deve ser excluído de uma atribuição.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d2484d601de3c200cfe300a77245e873502ecc0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42770120"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="2b8fa-103">Tipo de recurso exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2b8fa-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="2b8fa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2b8fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b8fa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b8fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b8fa-106">Representa um grupo que deve ser excluído de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="2b8fa-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="2b8fa-107">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="2b8fa-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2b8fa-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b8fa-108">Properties</span></span>
|<span data-ttu-id="2b8fa-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b8fa-109">Property</span></span>|<span data-ttu-id="2b8fa-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b8fa-110">Type</span></span>|<span data-ttu-id="2b8fa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b8fa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b8fa-112">groupId</span><span class="sxs-lookup"><span data-stu-id="2b8fa-112">groupId</span></span>|<span data-ttu-id="2b8fa-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b8fa-113">String</span></span>|<span data-ttu-id="2b8fa-114">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="2b8fa-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="2b8fa-115">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="2b8fa-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b8fa-116">Relações</span><span class="sxs-lookup"><span data-stu-id="2b8fa-116">Relationships</span></span>
<span data-ttu-id="2b8fa-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b8fa-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b8fa-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b8fa-118">JSON Representation</span></span>
<span data-ttu-id="2b8fa-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b8fa-119">Here is a JSON representation of the resource.</span></span>
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




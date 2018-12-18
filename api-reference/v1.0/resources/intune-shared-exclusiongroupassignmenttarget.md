---
title: Tipo de recurso exclusionGroupAssignmentTarget
description: Representa um grupo que deve ser excluído de uma atribuição.
author: tfitzmac
ms.openlocfilehash: 8193ac714f7f68dc371454c809c3eaa3176f8453
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304510"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="e8e7e-103">Tipo de recurso exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e8e7e-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="e8e7e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e8e7e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8e7e-105">Representa um grupo que deve ser excluído de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="e8e7e-105">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="e8e7e-106">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="e8e7e-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e8e7e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8e7e-107">Properties</span></span>
|<span data-ttu-id="e8e7e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8e7e-108">Property</span></span>|<span data-ttu-id="e8e7e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8e7e-109">Type</span></span>|<span data-ttu-id="e8e7e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8e7e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8e7e-111">groupId</span><span class="sxs-lookup"><span data-stu-id="e8e7e-111">groupId</span></span>|<span data-ttu-id="e8e7e-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8e7e-112">String</span></span>|<span data-ttu-id="e8e7e-113">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="e8e7e-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="e8e7e-114">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="e8e7e-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8e7e-115">Relações</span><span class="sxs-lookup"><span data-stu-id="e8e7e-115">Relationships</span></span>
<span data-ttu-id="e8e7e-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e8e7e-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e8e7e-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8e7e-117">JSON Representation</span></span>
<span data-ttu-id="e8e7e-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8e7e-118">Here is a JSON representation of the resource.</span></span>
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




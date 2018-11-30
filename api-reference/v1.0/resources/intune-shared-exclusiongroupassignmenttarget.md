---
title: Tipo de recurso exclusionGroupAssignmentTarget
description: Representa um grupo que deve ser excluído de uma atribuição.
ms.openlocfilehash: fdbb463687d75791965db2ef05abfea1a269d1a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006063"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="458b6-103">Tipo de recurso exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="458b6-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="458b6-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="458b6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="458b6-105">Representa um grupo que deve ser excluído de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="458b6-105">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="458b6-106">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="458b6-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="458b6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="458b6-107">Properties</span></span>
|<span data-ttu-id="458b6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="458b6-108">Property</span></span>|<span data-ttu-id="458b6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="458b6-109">Type</span></span>|<span data-ttu-id="458b6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="458b6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="458b6-111">groupId</span><span class="sxs-lookup"><span data-stu-id="458b6-111">groupId</span></span>|<span data-ttu-id="458b6-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="458b6-112">String</span></span>|<span data-ttu-id="458b6-113">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="458b6-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="458b6-114">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="458b6-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="458b6-115">Relações</span><span class="sxs-lookup"><span data-stu-id="458b6-115">Relationships</span></span>
<span data-ttu-id="458b6-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="458b6-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="458b6-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="458b6-117">JSON Representation</span></span>
<span data-ttu-id="458b6-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="458b6-118">Here is a JSON representation of the resource.</span></span>
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




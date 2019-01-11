---
title: Tipo de recurso exclusionGroupAssignmentTarget
description: Representa um grupo que deve ser excluído de uma atribuição.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ad844205e0cb5f5b4d0b86d71212e2d9c2ca223e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826450"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="4d2c8-103">Tipo de recurso exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4d2c8-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="4d2c8-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4d2c8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d2c8-105">Representa um grupo que deve ser excluído de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="4d2c8-105">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="4d2c8-106">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="4d2c8-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4d2c8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d2c8-107">Properties</span></span>
|<span data-ttu-id="4d2c8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d2c8-108">Property</span></span>|<span data-ttu-id="4d2c8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d2c8-109">Type</span></span>|<span data-ttu-id="4d2c8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d2c8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d2c8-111">groupId</span><span class="sxs-lookup"><span data-stu-id="4d2c8-111">groupId</span></span>|<span data-ttu-id="4d2c8-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d2c8-112">String</span></span>|<span data-ttu-id="4d2c8-113">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="4d2c8-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="4d2c8-114">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="4d2c8-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d2c8-115">Relações</span><span class="sxs-lookup"><span data-stu-id="4d2c8-115">Relationships</span></span>
<span data-ttu-id="4d2c8-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4d2c8-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4d2c8-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d2c8-117">JSON Representation</span></span>
<span data-ttu-id="4d2c8-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4d2c8-118">Here is a JSON representation of the resource.</span></span>
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




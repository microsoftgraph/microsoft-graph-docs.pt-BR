---
title: tipo de recurso variableManagementConditionExpression
description: Avalia o estado de condição de gerenciamento como uma expressão booleana.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8be06947bfce0e032965d3704ab9eec3a401845f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298754"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="3da13-103">tipo de recurso variableManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="3da13-103">variableManagementConditionExpression resource type</span></span>

<span data-ttu-id="3da13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3da13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3da13-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3da13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3da13-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3da13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3da13-107">Avalia o estado de condição de gerenciamento como uma expressão booleana.</span><span class="sxs-lookup"><span data-stu-id="3da13-107">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="3da13-108">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="3da13-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3da13-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3da13-109">Properties</span></span>
|<span data-ttu-id="3da13-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3da13-110">Property</span></span>|<span data-ttu-id="3da13-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3da13-111">Type</span></span>|<span data-ttu-id="3da13-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3da13-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3da13-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="3da13-113">managementConditionId</span></span>|<span data-ttu-id="3da13-114">String</span><span class="sxs-lookup"><span data-stu-id="3da13-114">String</span></span>|<span data-ttu-id="3da13-115">A ID da condição de gerenciamento usada para avaliar a expressão.</span><span class="sxs-lookup"><span data-stu-id="3da13-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3da13-116">Relações</span><span class="sxs-lookup"><span data-stu-id="3da13-116">Relationships</span></span>
<span data-ttu-id="3da13-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3da13-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3da13-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3da13-118">JSON Representation</span></span>
<span data-ttu-id="3da13-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3da13-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.variableManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.variableManagementConditionExpression",
  "managementConditionId": "String"
}
```





---
title: tipo de recurso unaryManagementConditionExpression
description: Uma expressão de condição de gerenciamento que é avaliada usando uma operação unário.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1f0bd5282307d1c8619f756d79209fb04a86bef2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453234"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="e6305-103">tipo de recurso unaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="e6305-103">unaryManagementConditionExpression resource type</span></span>

<span data-ttu-id="e6305-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6305-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6305-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e6305-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6305-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6305-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6305-107">Uma expressão de condição de gerenciamento que é avaliada usando uma operação unário.</span><span class="sxs-lookup"><span data-stu-id="e6305-107">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="e6305-108">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="e6305-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e6305-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6305-109">Properties</span></span>
|<span data-ttu-id="e6305-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6305-110">Property</span></span>|<span data-ttu-id="e6305-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6305-111">Type</span></span>|<span data-ttu-id="e6305-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6305-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6305-113">operator</span><span class="sxs-lookup"><span data-stu-id="e6305-113">operator</span></span>|[<span data-ttu-id="e6305-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="e6305-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="e6305-115">O operador usado na avaliação da operação unário.</span><span class="sxs-lookup"><span data-stu-id="e6305-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="e6305-116">Os valores possíveis são `not`:.</span><span class="sxs-lookup"><span data-stu-id="e6305-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="e6305-117">normaliza</span><span class="sxs-lookup"><span data-stu-id="e6305-117">operand</span></span>|[<span data-ttu-id="e6305-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="e6305-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="e6305-119">O operando da operação unário.</span><span class="sxs-lookup"><span data-stu-id="e6305-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6305-120">Relações</span><span class="sxs-lookup"><span data-stu-id="e6305-120">Relationships</span></span>
<span data-ttu-id="e6305-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6305-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6305-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6305-122">JSON Representation</span></span>
<span data-ttu-id="e6305-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6305-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unaryManagementConditionExpression",
  "operator": "String",
  "operand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```




---
title: tipo de recurso binaryManagementConditionExpression
description: Uma expressão de condição de gerenciamento que é avaliada usando uma operação binária.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d70306923b86f6d42942c5ce6b78ff31819d47d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150481"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="b4131-103">tipo de recurso binaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="b4131-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="b4131-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b4131-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4131-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4131-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4131-106">Uma expressão de condição de gerenciamento que é avaliada usando uma operação binária.</span><span class="sxs-lookup"><span data-stu-id="b4131-106">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="b4131-107">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="b4131-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b4131-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4131-108">Properties</span></span>
|<span data-ttu-id="b4131-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4131-109">Property</span></span>|<span data-ttu-id="b4131-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4131-110">Type</span></span>|<span data-ttu-id="b4131-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4131-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4131-112">operador</span><span class="sxs-lookup"><span data-stu-id="b4131-112">operator</span></span>|[<span data-ttu-id="b4131-113">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="b4131-113">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="b4131-114">O operador usado na avaliação da operação binária.</span><span class="sxs-lookup"><span data-stu-id="b4131-114">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="b4131-115">Os valores possíveis são: `or` e `and`.</span><span class="sxs-lookup"><span data-stu-id="b4131-115">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="b4131-116">firstOperand</span><span class="sxs-lookup"><span data-stu-id="b4131-116">firstOperand</span></span>|[<span data-ttu-id="b4131-117">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="b4131-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="b4131-118">O primeiro operando da operação binária.</span><span class="sxs-lookup"><span data-stu-id="b4131-118">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="b4131-119">secondOperand</span><span class="sxs-lookup"><span data-stu-id="b4131-119">secondOperand</span></span>|[<span data-ttu-id="b4131-120">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="b4131-120">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="b4131-121">O segundo operando da operação binária.</span><span class="sxs-lookup"><span data-stu-id="b4131-121">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4131-122">Relações</span><span class="sxs-lookup"><span data-stu-id="b4131-122">Relationships</span></span>
<span data-ttu-id="b4131-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4131-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4131-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4131-124">JSON Representation</span></span>
<span data-ttu-id="b4131-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4131-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.binaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.binaryManagementConditionExpression",
  "operator": "String",
  "firstOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  },
  "secondOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```





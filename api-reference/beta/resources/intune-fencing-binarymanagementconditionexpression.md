---
title: tipo de recurso de binaryManagementConditionExpression
description: Uma expressão de condição de gerenciamento que é avaliada usando uma operação de binário.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 509e03e7d492289fc9615f7f8ad47bf13d5bead4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857047"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="b06bc-103">tipo de recurso de binaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="b06bc-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="b06bc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b06bc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b06bc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b06bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b06bc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b06bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b06bc-107">Uma expressão de condição de gerenciamento que é avaliada usando uma operação de binário.</span><span class="sxs-lookup"><span data-stu-id="b06bc-107">A management condition expression that is evaluated using a binary operation.</span></span>

<span data-ttu-id="b06bc-108">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="b06bc-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b06bc-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b06bc-109">Properties</span></span>
|<span data-ttu-id="b06bc-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b06bc-110">Property</span></span>|<span data-ttu-id="b06bc-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b06bc-111">Type</span></span>|<span data-ttu-id="b06bc-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b06bc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b06bc-113">operador</span><span class="sxs-lookup"><span data-stu-id="b06bc-113">operator</span></span>|[<span data-ttu-id="b06bc-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="b06bc-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="b06bc-115">O operador usado na avaliação da operação binário.</span><span class="sxs-lookup"><span data-stu-id="b06bc-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="b06bc-116">Os valores possíveis são: `or` e `and`.</span><span class="sxs-lookup"><span data-stu-id="b06bc-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="b06bc-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="b06bc-117">firstOperand</span></span>|[<span data-ttu-id="b06bc-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="b06bc-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="b06bc-119">O primeiro operando da operação binário.</span><span class="sxs-lookup"><span data-stu-id="b06bc-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="b06bc-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="b06bc-120">secondOperand</span></span>|[<span data-ttu-id="b06bc-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="b06bc-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="b06bc-122">O segundo operando da operação binário.</span><span class="sxs-lookup"><span data-stu-id="b06bc-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b06bc-123">Relações</span><span class="sxs-lookup"><span data-stu-id="b06bc-123">Relationships</span></span>
<span data-ttu-id="b06bc-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b06bc-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b06bc-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b06bc-125">JSON Representation</span></span>
<span data-ttu-id="b06bc-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b06bc-126">Here is a JSON representation of the resource.</span></span>
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






---
title: tipo de recurso binaryManagementConditionExpression
description: Uma expressão de condição de gerenciamento que é avaliada usando uma operação binária.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 575f5d14b3c7427976814405729f12ed48d8a3fa
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442742"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="b4e0e-103">tipo de recurso binaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="b4e0e-103">binaryManagementConditionExpression resource type</span></span>

<span data-ttu-id="b4e0e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4e0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4e0e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b4e0e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4e0e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4e0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4e0e-107">Uma expressão de condição de gerenciamento que é avaliada usando uma operação binária.</span><span class="sxs-lookup"><span data-stu-id="b4e0e-107">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="b4e0e-108">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="b4e0e-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b4e0e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4e0e-109">Properties</span></span>
|<span data-ttu-id="b4e0e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4e0e-110">Property</span></span>|<span data-ttu-id="b4e0e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4e0e-111">Type</span></span>|<span data-ttu-id="b4e0e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4e0e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4e0e-113">operator</span><span class="sxs-lookup"><span data-stu-id="b4e0e-113">operator</span></span>|[<span data-ttu-id="b4e0e-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="b4e0e-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="b4e0e-115">O operador usado na avaliação da operação binária.</span><span class="sxs-lookup"><span data-stu-id="b4e0e-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="b4e0e-116">Os valores possíveis são: `or` e `and`.</span><span class="sxs-lookup"><span data-stu-id="b4e0e-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="b4e0e-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="b4e0e-117">firstOperand</span></span>|[<span data-ttu-id="b4e0e-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="b4e0e-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="b4e0e-119">O primeiro operando da operação binária.</span><span class="sxs-lookup"><span data-stu-id="b4e0e-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="b4e0e-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="b4e0e-120">secondOperand</span></span>|[<span data-ttu-id="b4e0e-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="b4e0e-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="b4e0e-122">O segundo operando da operação binária.</span><span class="sxs-lookup"><span data-stu-id="b4e0e-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4e0e-123">Relações</span><span class="sxs-lookup"><span data-stu-id="b4e0e-123">Relationships</span></span>
<span data-ttu-id="b4e0e-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4e0e-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4e0e-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4e0e-125">JSON Representation</span></span>
<span data-ttu-id="b4e0e-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4e0e-126">Here is a JSON representation of the resource.</span></span>
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




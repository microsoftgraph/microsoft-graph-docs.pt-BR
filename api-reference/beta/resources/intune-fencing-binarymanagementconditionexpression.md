---
title: tipo de recurso de binaryManagementConditionExpression
description: Uma expressão de condição de gerenciamento que é avaliada usando uma operação de binário.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 722387492e6167c3bd74d306fa03e4835bc12dbe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402724"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="c825a-103">tipo de recurso de binaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="c825a-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="c825a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c825a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c825a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c825a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c825a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c825a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c825a-107">Uma expressão de condição de gerenciamento que é avaliada usando uma operação de binário.</span><span class="sxs-lookup"><span data-stu-id="c825a-107">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="c825a-108">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="c825a-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c825a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c825a-109">Properties</span></span>
|<span data-ttu-id="c825a-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c825a-110">Property</span></span>|<span data-ttu-id="c825a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c825a-111">Type</span></span>|<span data-ttu-id="c825a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c825a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c825a-113">operador</span><span class="sxs-lookup"><span data-stu-id="c825a-113">operator</span></span>|[<span data-ttu-id="c825a-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="c825a-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="c825a-115">O operador usado na avaliação da operação binário.</span><span class="sxs-lookup"><span data-stu-id="c825a-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="c825a-116">Os valores possíveis são: `or` e `and`.</span><span class="sxs-lookup"><span data-stu-id="c825a-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="c825a-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="c825a-117">firstOperand</span></span>|[<span data-ttu-id="c825a-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="c825a-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="c825a-119">O primeiro operando da operação binário.</span><span class="sxs-lookup"><span data-stu-id="c825a-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="c825a-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="c825a-120">secondOperand</span></span>|[<span data-ttu-id="c825a-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="c825a-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="c825a-122">O segundo operando da operação binário.</span><span class="sxs-lookup"><span data-stu-id="c825a-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c825a-123">Relações</span><span class="sxs-lookup"><span data-stu-id="c825a-123">Relationships</span></span>
<span data-ttu-id="c825a-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c825a-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c825a-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c825a-125">JSON Representation</span></span>
<span data-ttu-id="c825a-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c825a-126">Here is a JSON representation of the resource.</span></span>
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





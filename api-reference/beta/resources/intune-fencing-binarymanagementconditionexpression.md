---
title: tipo de recurso de binaryManagementConditionExpression
description: Uma expressão de condição de gerenciamento que é avaliada usando uma operação de binário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b15938d0bb29fdfdad8abb1b37b02ad1e6468cf9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978533"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="ddbfe-103">tipo de recurso de binaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="ddbfe-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="ddbfe-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ddbfe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddbfe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ddbfe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ddbfe-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ddbfe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddbfe-107">Uma expressão de condição de gerenciamento que é avaliada usando uma operação de binário.</span><span class="sxs-lookup"><span data-stu-id="ddbfe-107">A management condition expression that is evaluated using a binary operation.</span></span>

<span data-ttu-id="ddbfe-108">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="ddbfe-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ddbfe-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ddbfe-109">Properties</span></span>
|<span data-ttu-id="ddbfe-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddbfe-110">Property</span></span>|<span data-ttu-id="ddbfe-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddbfe-111">Type</span></span>|<span data-ttu-id="ddbfe-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddbfe-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddbfe-113">operador</span><span class="sxs-lookup"><span data-stu-id="ddbfe-113">operator</span></span>|[<span data-ttu-id="ddbfe-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="ddbfe-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="ddbfe-115">O operador usado na avaliação da operação binário.</span><span class="sxs-lookup"><span data-stu-id="ddbfe-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="ddbfe-116">Os valores possíveis são: `or` e `and`.</span><span class="sxs-lookup"><span data-stu-id="ddbfe-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="ddbfe-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="ddbfe-117">firstOperand</span></span>|[<span data-ttu-id="ddbfe-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="ddbfe-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="ddbfe-119">O primeiro operando da operação binário.</span><span class="sxs-lookup"><span data-stu-id="ddbfe-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="ddbfe-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="ddbfe-120">secondOperand</span></span>|[<span data-ttu-id="ddbfe-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="ddbfe-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="ddbfe-122">O segundo operando da operação binário.</span><span class="sxs-lookup"><span data-stu-id="ddbfe-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddbfe-123">Relações</span><span class="sxs-lookup"><span data-stu-id="ddbfe-123">Relationships</span></span>
<span data-ttu-id="ddbfe-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ddbfe-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ddbfe-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ddbfe-125">JSON Representation</span></span>
<span data-ttu-id="ddbfe-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ddbfe-126">Here is a JSON representation of the resource.</span></span>
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






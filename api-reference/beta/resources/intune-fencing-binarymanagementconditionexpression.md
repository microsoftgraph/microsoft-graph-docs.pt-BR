---
title: tipo de recurso binaryManagementConditionExpression
description: Uma expressão de condição de gerenciamento que é avaliada usando uma operação binária.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97c812c3a26af0401bbdea87997167bcada05a37
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994815"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="da264-103">tipo de recurso binaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="da264-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="da264-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="da264-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da264-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="da264-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da264-106">Uma expressão de condição de gerenciamento que é avaliada usando uma operação binária.</span><span class="sxs-lookup"><span data-stu-id="da264-106">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="da264-107">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="da264-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="da264-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da264-108">Properties</span></span>
|<span data-ttu-id="da264-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da264-109">Property</span></span>|<span data-ttu-id="da264-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="da264-110">Type</span></span>|<span data-ttu-id="da264-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="da264-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da264-112">operator</span><span class="sxs-lookup"><span data-stu-id="da264-112">operator</span></span>|[<span data-ttu-id="da264-113">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="da264-113">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="da264-114">O operador usado na avaliação da operação binária.</span><span class="sxs-lookup"><span data-stu-id="da264-114">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="da264-115">Os valores possíveis são: `or` e `and`.</span><span class="sxs-lookup"><span data-stu-id="da264-115">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="da264-116">firstOperand</span><span class="sxs-lookup"><span data-stu-id="da264-116">firstOperand</span></span>|[<span data-ttu-id="da264-117">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="da264-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="da264-118">O primeiro operando da operação binária.</span><span class="sxs-lookup"><span data-stu-id="da264-118">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="da264-119">secondOperand</span><span class="sxs-lookup"><span data-stu-id="da264-119">secondOperand</span></span>|[<span data-ttu-id="da264-120">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="da264-120">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="da264-121">O segundo operando da operação binária.</span><span class="sxs-lookup"><span data-stu-id="da264-121">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da264-122">Relações</span><span class="sxs-lookup"><span data-stu-id="da264-122">Relationships</span></span>
<span data-ttu-id="da264-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da264-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da264-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da264-124">JSON Representation</span></span>
<span data-ttu-id="da264-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da264-125">Here is a JSON representation of the resource.</span></span>
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






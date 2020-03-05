---
title: tipo de recurso binaryManagementConditionExpression
description: Uma expressão de condição de gerenciamento que é avaliada usando uma operação binária.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d0919ac70a5855900aef5f87ad5f63e35e28b60a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528199"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="7ff5a-103">tipo de recurso binaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="7ff5a-103">binaryManagementConditionExpression resource type</span></span>

<span data-ttu-id="7ff5a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7ff5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ff5a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ff5a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ff5a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ff5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ff5a-107">Uma expressão de condição de gerenciamento que é avaliada usando uma operação binária.</span><span class="sxs-lookup"><span data-stu-id="7ff5a-107">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="7ff5a-108">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="7ff5a-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7ff5a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ff5a-109">Properties</span></span>
|<span data-ttu-id="7ff5a-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ff5a-110">Property</span></span>|<span data-ttu-id="7ff5a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ff5a-111">Type</span></span>|<span data-ttu-id="7ff5a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ff5a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ff5a-113">operator</span><span class="sxs-lookup"><span data-stu-id="7ff5a-113">operator</span></span>|[<span data-ttu-id="7ff5a-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="7ff5a-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="7ff5a-115">O operador usado na avaliação da operação binária.</span><span class="sxs-lookup"><span data-stu-id="7ff5a-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="7ff5a-116">Os valores possíveis são: `or` e `and`.</span><span class="sxs-lookup"><span data-stu-id="7ff5a-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="7ff5a-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="7ff5a-117">firstOperand</span></span>|[<span data-ttu-id="7ff5a-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="7ff5a-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="7ff5a-119">O primeiro operando da operação binária.</span><span class="sxs-lookup"><span data-stu-id="7ff5a-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="7ff5a-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="7ff5a-120">secondOperand</span></span>|[<span data-ttu-id="7ff5a-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="7ff5a-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="7ff5a-122">O segundo operando da operação binária.</span><span class="sxs-lookup"><span data-stu-id="7ff5a-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ff5a-123">Relações</span><span class="sxs-lookup"><span data-stu-id="7ff5a-123">Relationships</span></span>
<span data-ttu-id="7ff5a-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ff5a-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ff5a-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ff5a-125">JSON Representation</span></span>
<span data-ttu-id="7ff5a-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ff5a-126">Here is a JSON representation of the resource.</span></span>
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




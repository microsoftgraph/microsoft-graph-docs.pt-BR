---
title: tipo de recurso unaryManagementConditionExpression
description: Uma expressão de condição de gerenciamento que é avaliada usando uma operação unário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eee7a423ca412eb4ee86e3f0b5a5f13ec786a690
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941195"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="62dd5-103">tipo de recurso unaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="62dd5-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="62dd5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62dd5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62dd5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62dd5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62dd5-106">Uma expressão de condição de gerenciamento que é avaliada usando uma operação unário.</span><span class="sxs-lookup"><span data-stu-id="62dd5-106">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="62dd5-107">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="62dd5-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="62dd5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62dd5-108">Properties</span></span>
|<span data-ttu-id="62dd5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62dd5-109">Property</span></span>|<span data-ttu-id="62dd5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="62dd5-110">Type</span></span>|<span data-ttu-id="62dd5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="62dd5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62dd5-112">operator</span><span class="sxs-lookup"><span data-stu-id="62dd5-112">operator</span></span>|[<span data-ttu-id="62dd5-113">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="62dd5-113">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="62dd5-114">O operador usado na avaliação da operação unário.</span><span class="sxs-lookup"><span data-stu-id="62dd5-114">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="62dd5-115">Os valores possíveis são `not`:.</span><span class="sxs-lookup"><span data-stu-id="62dd5-115">Possible values are: `not`.</span></span>|
|<span data-ttu-id="62dd5-116">normaliza</span><span class="sxs-lookup"><span data-stu-id="62dd5-116">operand</span></span>|[<span data-ttu-id="62dd5-117">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="62dd5-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="62dd5-118">O operando da operação unário.</span><span class="sxs-lookup"><span data-stu-id="62dd5-118">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62dd5-119">Relações</span><span class="sxs-lookup"><span data-stu-id="62dd5-119">Relationships</span></span>
<span data-ttu-id="62dd5-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="62dd5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62dd5-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62dd5-121">JSON Representation</span></span>
<span data-ttu-id="62dd5-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62dd5-122">Here is a JSON representation of the resource.</span></span>
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





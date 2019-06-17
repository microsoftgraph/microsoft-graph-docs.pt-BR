---
title: tipo de recurso unaryManagementConditionExpression
description: Uma expressão de condição de gerenciamento que é avaliada usando uma operação unário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5eb5e7ed67b0731cc795ab791c2463294764ead6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990103"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="750ab-103">tipo de recurso unaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="750ab-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="750ab-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="750ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="750ab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="750ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="750ab-106">Uma expressão de condição de gerenciamento que é avaliada usando uma operação unário.</span><span class="sxs-lookup"><span data-stu-id="750ab-106">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="750ab-107">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="750ab-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="750ab-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="750ab-108">Properties</span></span>
|<span data-ttu-id="750ab-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="750ab-109">Property</span></span>|<span data-ttu-id="750ab-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="750ab-110">Type</span></span>|<span data-ttu-id="750ab-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="750ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="750ab-112">operator</span><span class="sxs-lookup"><span data-stu-id="750ab-112">operator</span></span>|[<span data-ttu-id="750ab-113">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="750ab-113">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="750ab-114">O operador usado na avaliação da operação unário.</span><span class="sxs-lookup"><span data-stu-id="750ab-114">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="750ab-115">Os valores possíveis são `not`:.</span><span class="sxs-lookup"><span data-stu-id="750ab-115">Possible values are: `not`.</span></span>|
|<span data-ttu-id="750ab-116">normaliza</span><span class="sxs-lookup"><span data-stu-id="750ab-116">operand</span></span>|[<span data-ttu-id="750ab-117">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="750ab-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="750ab-118">O operando da operação unário.</span><span class="sxs-lookup"><span data-stu-id="750ab-118">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="750ab-119">Relações</span><span class="sxs-lookup"><span data-stu-id="750ab-119">Relationships</span></span>
<span data-ttu-id="750ab-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="750ab-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="750ab-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="750ab-121">JSON Representation</span></span>
<span data-ttu-id="750ab-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="750ab-122">Here is a JSON representation of the resource.</span></span>
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






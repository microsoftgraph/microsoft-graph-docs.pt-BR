---
title: tipo de recurso unaryManagementConditionExpression
description: Uma expressão de condição de gerenciamento que é avaliada usando uma operação unário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 155386e63a5d1f28a3cbe0ed35b9c5f659389bc6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011061"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="00081-103">tipo de recurso unaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="00081-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="00081-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="00081-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00081-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="00081-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00081-106">Uma expressão de condição de gerenciamento que é avaliada usando uma operação unário.</span><span class="sxs-lookup"><span data-stu-id="00081-106">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="00081-107">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="00081-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="00081-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00081-108">Properties</span></span>
|<span data-ttu-id="00081-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00081-109">Property</span></span>|<span data-ttu-id="00081-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="00081-110">Type</span></span>|<span data-ttu-id="00081-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="00081-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00081-112">operator</span><span class="sxs-lookup"><span data-stu-id="00081-112">operator</span></span>|[<span data-ttu-id="00081-113">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="00081-113">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="00081-114">O operador usado na avaliação da operação unário.</span><span class="sxs-lookup"><span data-stu-id="00081-114">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="00081-115">Os valores possíveis são `not`:.</span><span class="sxs-lookup"><span data-stu-id="00081-115">Possible values are: `not`.</span></span>|
|<span data-ttu-id="00081-116">normaliza</span><span class="sxs-lookup"><span data-stu-id="00081-116">operand</span></span>|[<span data-ttu-id="00081-117">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="00081-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="00081-118">O operando da operação unário.</span><span class="sxs-lookup"><span data-stu-id="00081-118">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00081-119">Relações</span><span class="sxs-lookup"><span data-stu-id="00081-119">Relationships</span></span>
<span data-ttu-id="00081-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="00081-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00081-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00081-121">JSON Representation</span></span>
<span data-ttu-id="00081-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00081-122">Here is a JSON representation of the resource.</span></span>
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






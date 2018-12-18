---
title: tipo de recurso de unaryManagementConditionExpression
description: Uma expressão de condição de gerenciamento que é avaliada usando uma operação unária.
author: tfitzmac
ms.openlocfilehash: 43711e68d88bdf0854e8501377fbf3e30b25b3ec
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344342"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="bb81d-103">tipo de recurso de unaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="bb81d-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="bb81d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bb81d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb81d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bb81d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb81d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bb81d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb81d-107">Uma expressão de condição de gerenciamento que é avaliada usando uma operação unária.</span><span class="sxs-lookup"><span data-stu-id="bb81d-107">A management condition expression that is evaluated using a unary operation.</span></span>

<span data-ttu-id="bb81d-108">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="bb81d-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bb81d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb81d-109">Properties</span></span>
|<span data-ttu-id="bb81d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb81d-110">Property</span></span>|<span data-ttu-id="bb81d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb81d-111">Type</span></span>|<span data-ttu-id="bb81d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb81d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb81d-113">operador</span><span class="sxs-lookup"><span data-stu-id="bb81d-113">operator</span></span>|[<span data-ttu-id="bb81d-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="bb81d-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="bb81d-115">O operador usado na avaliação da operação unário.</span><span class="sxs-lookup"><span data-stu-id="bb81d-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="bb81d-116">Os valores possíveis são: `not`.</span><span class="sxs-lookup"><span data-stu-id="bb81d-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="bb81d-117">operando</span><span class="sxs-lookup"><span data-stu-id="bb81d-117">operand</span></span>|[<span data-ttu-id="bb81d-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="bb81d-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="bb81d-119">O operando da operação unário.</span><span class="sxs-lookup"><span data-stu-id="bb81d-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb81d-120">Relações</span><span class="sxs-lookup"><span data-stu-id="bb81d-120">Relationships</span></span>
<span data-ttu-id="bb81d-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb81d-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bb81d-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb81d-122">JSON Representation</span></span>
<span data-ttu-id="bb81d-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb81d-123">Here is a JSON representation of the resource.</span></span>
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






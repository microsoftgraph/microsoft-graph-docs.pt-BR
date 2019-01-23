---
title: tipo de recurso de unaryManagementConditionExpression
description: Uma expressão de condição de gerenciamento que é avaliada usando uma operação unária.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f1224a869ec2ec9cae2f38273f7a68b64d3d7333
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406777"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="91bdc-103">tipo de recurso de unaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="91bdc-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="91bdc-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="91bdc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="91bdc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="91bdc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91bdc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="91bdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91bdc-107">Uma expressão de condição de gerenciamento que é avaliada usando uma operação unária.</span><span class="sxs-lookup"><span data-stu-id="91bdc-107">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="91bdc-108">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="91bdc-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="91bdc-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91bdc-109">Properties</span></span>
|<span data-ttu-id="91bdc-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91bdc-110">Property</span></span>|<span data-ttu-id="91bdc-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="91bdc-111">Type</span></span>|<span data-ttu-id="91bdc-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="91bdc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91bdc-113">operador</span><span class="sxs-lookup"><span data-stu-id="91bdc-113">operator</span></span>|[<span data-ttu-id="91bdc-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="91bdc-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="91bdc-115">O operador usado na avaliação da operação unário.</span><span class="sxs-lookup"><span data-stu-id="91bdc-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="91bdc-116">Os valores possíveis são: `not`.</span><span class="sxs-lookup"><span data-stu-id="91bdc-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="91bdc-117">operando</span><span class="sxs-lookup"><span data-stu-id="91bdc-117">operand</span></span>|[<span data-ttu-id="91bdc-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="91bdc-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="91bdc-119">O operando da operação unário.</span><span class="sxs-lookup"><span data-stu-id="91bdc-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91bdc-120">Relações</span><span class="sxs-lookup"><span data-stu-id="91bdc-120">Relationships</span></span>
<span data-ttu-id="91bdc-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="91bdc-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91bdc-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91bdc-122">JSON Representation</span></span>
<span data-ttu-id="91bdc-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91bdc-123">Here is a JSON representation of the resource.</span></span>
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





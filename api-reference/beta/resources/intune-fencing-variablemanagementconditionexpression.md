---
title: tipo de recurso de variableManagementConditionExpression
description: Avalia o estado de condição de gerenciamento como uma expressão booleana.
ms.openlocfilehash: 220cb54680755461edb9dab6edf076f8ae0c6a68
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037474"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="94dd5-103">tipo de recurso de variableManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="94dd5-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="94dd5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="94dd5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94dd5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="94dd5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94dd5-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="94dd5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94dd5-107">Avalia o estado de condição de gerenciamento como uma expressão booleana.</span><span class="sxs-lookup"><span data-stu-id="94dd5-107">Evaluates the management condition state as a Boolean expression.</span></span>

<span data-ttu-id="94dd5-108">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="94dd5-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="94dd5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94dd5-109">Properties</span></span>
|<span data-ttu-id="94dd5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94dd5-110">Property</span></span>|<span data-ttu-id="94dd5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="94dd5-111">Type</span></span>|<span data-ttu-id="94dd5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="94dd5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94dd5-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="94dd5-113">managementConditionId</span></span>|<span data-ttu-id="94dd5-114">String</span><span class="sxs-lookup"><span data-stu-id="94dd5-114">String</span></span>|<span data-ttu-id="94dd5-115">A id de condição de gerenciamento que é usada para avaliar a expressão.</span><span class="sxs-lookup"><span data-stu-id="94dd5-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94dd5-116">Relações</span><span class="sxs-lookup"><span data-stu-id="94dd5-116">Relationships</span></span>
<span data-ttu-id="94dd5-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94dd5-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="94dd5-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94dd5-118">JSON Representation</span></span>
<span data-ttu-id="94dd5-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94dd5-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.variableManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.variableManagementConditionExpression",
  "managementConditionId": "String"
}
```






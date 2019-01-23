---
title: tipo de recurso de variableManagementConditionExpression
description: Avalia o estado de condição de gerenciamento como uma expressão booleana.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6a5e7efd0c8213f40d1dfb5f86d2f86c999069d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399623"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="60918-103">tipo de recurso de variableManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="60918-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="60918-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="60918-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="60918-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="60918-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60918-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="60918-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60918-107">Avalia o estado de condição de gerenciamento como uma expressão booleana.</span><span class="sxs-lookup"><span data-stu-id="60918-107">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="60918-108">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="60918-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="60918-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60918-109">Properties</span></span>
|<span data-ttu-id="60918-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60918-110">Property</span></span>|<span data-ttu-id="60918-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="60918-111">Type</span></span>|<span data-ttu-id="60918-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="60918-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60918-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="60918-113">managementConditionId</span></span>|<span data-ttu-id="60918-114">String</span><span class="sxs-lookup"><span data-stu-id="60918-114">String</span></span>|<span data-ttu-id="60918-115">A id de condição de gerenciamento que é usada para avaliar a expressão.</span><span class="sxs-lookup"><span data-stu-id="60918-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60918-116">Relações</span><span class="sxs-lookup"><span data-stu-id="60918-116">Relationships</span></span>
<span data-ttu-id="60918-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="60918-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60918-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60918-118">JSON Representation</span></span>
<span data-ttu-id="60918-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60918-119">Here is a JSON representation of the resource.</span></span>
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





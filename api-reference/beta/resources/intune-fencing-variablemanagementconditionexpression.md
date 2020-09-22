---
title: tipo de recurso variableManagementConditionExpression
description: Avalia o estado de condição de gerenciamento como uma expressão booleana.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2cb61473401d868fb98a9ea041f268252168d5be
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031239"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="6ebfc-103">tipo de recurso variableManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="6ebfc-103">variableManagementConditionExpression resource type</span></span>

<span data-ttu-id="6ebfc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ebfc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ebfc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ebfc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ebfc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ebfc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ebfc-107">Avalia o estado de condição de gerenciamento como uma expressão booleana.</span><span class="sxs-lookup"><span data-stu-id="6ebfc-107">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="6ebfc-108">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="6ebfc-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6ebfc-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6ebfc-109">Properties</span></span>
|<span data-ttu-id="6ebfc-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ebfc-110">Property</span></span>|<span data-ttu-id="6ebfc-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ebfc-111">Type</span></span>|<span data-ttu-id="6ebfc-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ebfc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ebfc-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="6ebfc-113">managementConditionId</span></span>|<span data-ttu-id="6ebfc-114">String</span><span class="sxs-lookup"><span data-stu-id="6ebfc-114">String</span></span>|<span data-ttu-id="6ebfc-115">A ID da condição de gerenciamento usada para avaliar a expressão.</span><span class="sxs-lookup"><span data-stu-id="6ebfc-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ebfc-116">Relações</span><span class="sxs-lookup"><span data-stu-id="6ebfc-116">Relationships</span></span>
<span data-ttu-id="6ebfc-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ebfc-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ebfc-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ebfc-118">JSON Representation</span></span>
<span data-ttu-id="6ebfc-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6ebfc-119">Here is a JSON representation of the resource.</span></span>
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







---
title: tipo de recurso variableManagementConditionExpression
description: Avalia o estado de condição de gerenciamento como uma expressão booleana.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8f091be4d717d57e447eacce08fb0a24905f1c14
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011047"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="511d7-103">tipo de recurso variableManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="511d7-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="511d7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="511d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="511d7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="511d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="511d7-106">Avalia o estado de condição de gerenciamento como uma expressão booleana.</span><span class="sxs-lookup"><span data-stu-id="511d7-106">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="511d7-107">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="511d7-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="511d7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="511d7-108">Properties</span></span>
|<span data-ttu-id="511d7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="511d7-109">Property</span></span>|<span data-ttu-id="511d7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="511d7-110">Type</span></span>|<span data-ttu-id="511d7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="511d7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="511d7-112">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="511d7-112">managementConditionId</span></span>|<span data-ttu-id="511d7-113">String</span><span class="sxs-lookup"><span data-stu-id="511d7-113">String</span></span>|<span data-ttu-id="511d7-114">A ID da condição de gerenciamento usada para avaliar a expressão.</span><span class="sxs-lookup"><span data-stu-id="511d7-114">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="511d7-115">Relações</span><span class="sxs-lookup"><span data-stu-id="511d7-115">Relationships</span></span>
<span data-ttu-id="511d7-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="511d7-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="511d7-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="511d7-117">JSON Representation</span></span>
<span data-ttu-id="511d7-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="511d7-118">Here is a JSON representation of the resource.</span></span>
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






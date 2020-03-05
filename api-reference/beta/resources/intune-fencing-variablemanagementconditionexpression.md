---
title: tipo de recurso variableManagementConditionExpression
description: Avalia o estado de condição de gerenciamento como uma expressão booleana.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 11c85ab4f2488c7cb27ae8564f49ab6a4faef585
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524487"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="4e66c-103">tipo de recurso variableManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="4e66c-103">variableManagementConditionExpression resource type</span></span>

<span data-ttu-id="4e66c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4e66c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e66c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e66c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e66c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e66c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e66c-107">Avalia o estado de condição de gerenciamento como uma expressão booleana.</span><span class="sxs-lookup"><span data-stu-id="4e66c-107">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="4e66c-108">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="4e66c-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4e66c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e66c-109">Properties</span></span>
|<span data-ttu-id="4e66c-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e66c-110">Property</span></span>|<span data-ttu-id="4e66c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e66c-111">Type</span></span>|<span data-ttu-id="4e66c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e66c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e66c-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="4e66c-113">managementConditionId</span></span>|<span data-ttu-id="4e66c-114">String</span><span class="sxs-lookup"><span data-stu-id="4e66c-114">String</span></span>|<span data-ttu-id="4e66c-115">A ID da condição de gerenciamento usada para avaliar a expressão.</span><span class="sxs-lookup"><span data-stu-id="4e66c-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e66c-116">Relações</span><span class="sxs-lookup"><span data-stu-id="4e66c-116">Relationships</span></span>
<span data-ttu-id="4e66c-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e66c-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e66c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e66c-118">JSON Representation</span></span>
<span data-ttu-id="4e66c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e66c-119">Here is a JSON representation of the resource.</span></span>
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




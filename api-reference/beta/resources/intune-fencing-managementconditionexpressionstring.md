---
title: tipo de recurso managementConditionExpressionString
description: Uma sequência de expressão de condição de gerenciamento é uma representação de cadeia de caracteres de uma expressão de condição de gerenciamento.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4b77be0d5f59dc1cd681104efb0c0404746e574
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528174"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="7ac0e-103">tipo de recurso managementConditionExpressionString</span><span class="sxs-lookup"><span data-stu-id="7ac0e-103">managementConditionExpressionString resource type</span></span>

<span data-ttu-id="7ac0e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7ac0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ac0e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ac0e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ac0e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ac0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ac0e-107">Uma sequência de expressão de condição de gerenciamento é uma representação de cadeia de caracteres de uma expressão de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="7ac0e-107">A management condition expression string is a string representation of a management condition expression.</span></span>


<span data-ttu-id="7ac0e-108">Herda de [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="7ac0e-108">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7ac0e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ac0e-109">Properties</span></span>
|<span data-ttu-id="7ac0e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ac0e-110">Property</span></span>|<span data-ttu-id="7ac0e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ac0e-111">Type</span></span>|<span data-ttu-id="7ac0e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ac0e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ac0e-113">valor</span><span class="sxs-lookup"><span data-stu-id="7ac0e-113">value</span></span>|<span data-ttu-id="7ac0e-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac0e-114">String</span></span>|<span data-ttu-id="7ac0e-115">O valor da cadeia de caracteres da expressão da declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="7ac0e-115">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ac0e-116">Relações</span><span class="sxs-lookup"><span data-stu-id="7ac0e-116">Relationships</span></span>
<span data-ttu-id="7ac0e-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ac0e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ac0e-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ac0e-118">JSON Representation</span></span>
<span data-ttu-id="7ac0e-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ac0e-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementConditionExpressionString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionExpressionString",
  "value": "String"
}
```




---
title: tipo de recurso managementConditionExpressionString
description: Uma sequência de expressão de condição de gerenciamento é uma representação de cadeia de caracteres de uma expressão de condição de gerenciamento.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3dac405c71e4e85cc29bb36d335a57bb51fbe0f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568728"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="3681b-103">tipo de recurso managementConditionExpressionString</span><span class="sxs-lookup"><span data-stu-id="3681b-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="3681b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3681b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3681b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3681b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3681b-106">Uma sequência de expressão de condição de gerenciamento é uma representação de cadeia de caracteres de uma expressão de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="3681b-106">A management condition expression string is a string representation of a management condition expression.</span></span>


<span data-ttu-id="3681b-107">Herda de [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="3681b-107">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3681b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3681b-108">Properties</span></span>
|<span data-ttu-id="3681b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3681b-109">Property</span></span>|<span data-ttu-id="3681b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3681b-110">Type</span></span>|<span data-ttu-id="3681b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3681b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3681b-112">valor</span><span class="sxs-lookup"><span data-stu-id="3681b-112">value</span></span>|<span data-ttu-id="3681b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3681b-113">String</span></span>|<span data-ttu-id="3681b-114">O valor da cadeia de caracteres da expressão da declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="3681b-114">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3681b-115">Relações</span><span class="sxs-lookup"><span data-stu-id="3681b-115">Relationships</span></span>
<span data-ttu-id="3681b-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3681b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3681b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3681b-117">JSON Representation</span></span>
<span data-ttu-id="3681b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3681b-118">Here is a JSON representation of the resource.</span></span>
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






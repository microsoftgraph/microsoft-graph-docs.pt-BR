---
title: tipo de recurso win32LobAppProductCodeRule
description: Um tipo complexo para armazenar o código do produto e os dados da regra de versão para um aplicativo LOB Win32. Essa regra não é suportada como uma regra de requisito.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd3dde2386c76b5ed7dee6174789667d44839c58
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790814"
---
# <a name="win32lobappproductcoderule-resource-type"></a><span data-ttu-id="36b00-104">tipo de recurso win32LobAppProductCodeRule</span><span class="sxs-lookup"><span data-stu-id="36b00-104">win32LobAppProductCodeRule resource type</span></span>

<span data-ttu-id="36b00-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36b00-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36b00-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="36b00-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36b00-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="36b00-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36b00-108">Um tipo complexo para armazenar o código do produto e os dados da regra de versão para um aplicativo LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="36b00-108">A complex type to store the product code and version rule data for a Win32 LOB app.</span></span> <span data-ttu-id="36b00-109">Essa regra não é suportada como uma regra de requisito.</span><span class="sxs-lookup"><span data-stu-id="36b00-109">This rule is not supported as a requirement rule.</span></span>


<span data-ttu-id="36b00-110">Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="36b00-110">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="36b00-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36b00-111">Properties</span></span>
|<span data-ttu-id="36b00-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36b00-112">Property</span></span>|<span data-ttu-id="36b00-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="36b00-113">Type</span></span>|<span data-ttu-id="36b00-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="36b00-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36b00-115">ruleType</span><span class="sxs-lookup"><span data-stu-id="36b00-115">ruleType</span></span>|[<span data-ttu-id="36b00-116">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="36b00-116">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="36b00-117">O tipo de regra que indica o objetivo da regra.</span><span class="sxs-lookup"><span data-stu-id="36b00-117">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="36b00-118">Herdado de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="36b00-118">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="36b00-119">Os valores possíveis são: `detection` e `requirement`.</span><span class="sxs-lookup"><span data-stu-id="36b00-119">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="36b00-120">productCode</span><span class="sxs-lookup"><span data-stu-id="36b00-120">productCode</span></span>|<span data-ttu-id="36b00-121">String</span><span class="sxs-lookup"><span data-stu-id="36b00-121">String</span></span>|<span data-ttu-id="36b00-122">O código do produto do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="36b00-122">The product code of the app.</span></span>|
|<span data-ttu-id="36b00-123">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="36b00-123">productVersionOperator</span></span>|[<span data-ttu-id="36b00-124">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="36b00-124">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="36b00-125">O operador de comparação de versão do produto.</span><span class="sxs-lookup"><span data-stu-id="36b00-125">The product version comparison operator.</span></span> <span data-ttu-id="36b00-126">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="36b00-126">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="36b00-127">productVersion</span><span class="sxs-lookup"><span data-stu-id="36b00-127">productVersion</span></span>|<span data-ttu-id="36b00-128">String</span><span class="sxs-lookup"><span data-stu-id="36b00-128">String</span></span>|<span data-ttu-id="36b00-129">O valor de comparação da versão do produto.</span><span class="sxs-lookup"><span data-stu-id="36b00-129">The product version comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36b00-130">Relações</span><span class="sxs-lookup"><span data-stu-id="36b00-130">Relationships</span></span>
<span data-ttu-id="36b00-131">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="36b00-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36b00-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36b00-132">JSON Representation</span></span>
<span data-ttu-id="36b00-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36b00-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppProductCodeRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppProductCodeRule",
  "ruleType": "String",
  "productCode": "String",
  "productVersionOperator": "String",
  "productVersion": "String"
}
```




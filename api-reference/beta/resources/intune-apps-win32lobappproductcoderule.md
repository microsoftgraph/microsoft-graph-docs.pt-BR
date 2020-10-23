---
title: tipo de recurso win32LobAppProductCodeRule
description: Um tipo complexo para armazenar o código do produto e os dados da regra de versão para um aplicativo LOB Win32. Essa regra não é suportada como uma regra de requisito.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ef52decf1cb85e1a850faf50ef29b3e9478a95fd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706237"
---
# <a name="win32lobappproductcoderule-resource-type"></a><span data-ttu-id="4ef1b-104">tipo de recurso win32LobAppProductCodeRule</span><span class="sxs-lookup"><span data-stu-id="4ef1b-104">win32LobAppProductCodeRule resource type</span></span>

<span data-ttu-id="4ef1b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ef1b-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ef1b-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4ef1b-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ef1b-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ef1b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ef1b-108">Um tipo complexo para armazenar o código do produto e os dados da regra de versão para um aplicativo LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="4ef1b-108">A complex type to store the product code and version rule data for a Win32 LOB app.</span></span> <span data-ttu-id="4ef1b-109">Essa regra não é suportada como uma regra de requisito.</span><span class="sxs-lookup"><span data-stu-id="4ef1b-109">This rule is not supported as a requirement rule.</span></span>


<span data-ttu-id="4ef1b-110">Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="4ef1b-110">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4ef1b-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ef1b-111">Properties</span></span>
|<span data-ttu-id="4ef1b-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ef1b-112">Property</span></span>|<span data-ttu-id="4ef1b-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ef1b-113">Type</span></span>|<span data-ttu-id="4ef1b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ef1b-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ef1b-115">ruleType</span><span class="sxs-lookup"><span data-stu-id="4ef1b-115">ruleType</span></span>|[<span data-ttu-id="4ef1b-116">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="4ef1b-116">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="4ef1b-117">O tipo de regra que indica o objetivo da regra.</span><span class="sxs-lookup"><span data-stu-id="4ef1b-117">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="4ef1b-118">Herdado de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="4ef1b-118">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="4ef1b-119">Os valores possíveis são: `detection` e `requirement`.</span><span class="sxs-lookup"><span data-stu-id="4ef1b-119">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="4ef1b-120">productCode</span><span class="sxs-lookup"><span data-stu-id="4ef1b-120">productCode</span></span>|<span data-ttu-id="4ef1b-121">String</span><span class="sxs-lookup"><span data-stu-id="4ef1b-121">String</span></span>|<span data-ttu-id="4ef1b-122">O código do produto do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4ef1b-122">The product code of the app.</span></span>|
|<span data-ttu-id="4ef1b-123">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="4ef1b-123">productVersionOperator</span></span>|[<span data-ttu-id="4ef1b-124">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="4ef1b-124">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="4ef1b-125">O operador de comparação de versão do produto.</span><span class="sxs-lookup"><span data-stu-id="4ef1b-125">The product version comparison operator.</span></span> <span data-ttu-id="4ef1b-126">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="4ef1b-126">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="4ef1b-127">productVersion</span><span class="sxs-lookup"><span data-stu-id="4ef1b-127">productVersion</span></span>|<span data-ttu-id="4ef1b-128">String</span><span class="sxs-lookup"><span data-stu-id="4ef1b-128">String</span></span>|<span data-ttu-id="4ef1b-129">O valor de comparação da versão do produto.</span><span class="sxs-lookup"><span data-stu-id="4ef1b-129">The product version comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ef1b-130">Relações</span><span class="sxs-lookup"><span data-stu-id="4ef1b-130">Relationships</span></span>
<span data-ttu-id="4ef1b-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ef1b-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ef1b-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ef1b-132">JSON Representation</span></span>
<span data-ttu-id="4ef1b-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ef1b-133">Here is a JSON representation of the resource.</span></span>
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






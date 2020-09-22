---
title: tipo de recurso win32LobAppProductCodeRule
description: Um tipo complexo para armazenar o código do produto e os dados da regra de versão para um aplicativo LOB Win32. Essa regra não é suportada como uma regra de requisito.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 11990f4deddb7bf29b9b447ae65e1903f6ecbc2d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092801"
---
# <a name="win32lobappproductcoderule-resource-type"></a><span data-ttu-id="089bf-104">tipo de recurso win32LobAppProductCodeRule</span><span class="sxs-lookup"><span data-stu-id="089bf-104">win32LobAppProductCodeRule resource type</span></span>

<span data-ttu-id="089bf-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="089bf-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="089bf-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="089bf-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="089bf-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="089bf-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="089bf-108">Um tipo complexo para armazenar o código do produto e os dados da regra de versão para um aplicativo LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="089bf-108">A complex type to store the product code and version rule data for a Win32 LOB app.</span></span> <span data-ttu-id="089bf-109">Essa regra não é suportada como uma regra de requisito.</span><span class="sxs-lookup"><span data-stu-id="089bf-109">This rule is not supported as a requirement rule.</span></span>


<span data-ttu-id="089bf-110">Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="089bf-110">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="089bf-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="089bf-111">Properties</span></span>
|<span data-ttu-id="089bf-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="089bf-112">Property</span></span>|<span data-ttu-id="089bf-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="089bf-113">Type</span></span>|<span data-ttu-id="089bf-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="089bf-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="089bf-115">ruleType</span><span class="sxs-lookup"><span data-stu-id="089bf-115">ruleType</span></span>|[<span data-ttu-id="089bf-116">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="089bf-116">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="089bf-117">O tipo de regra que indica o objetivo da regra.</span><span class="sxs-lookup"><span data-stu-id="089bf-117">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="089bf-118">Herdado de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="089bf-118">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="089bf-119">Os valores possíveis são: `detection` e `requirement`.</span><span class="sxs-lookup"><span data-stu-id="089bf-119">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="089bf-120">productCode</span><span class="sxs-lookup"><span data-stu-id="089bf-120">productCode</span></span>|<span data-ttu-id="089bf-121">String</span><span class="sxs-lookup"><span data-stu-id="089bf-121">String</span></span>|<span data-ttu-id="089bf-122">O código do produto do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="089bf-122">The product code of the app.</span></span>|
|<span data-ttu-id="089bf-123">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="089bf-123">productVersionOperator</span></span>|[<span data-ttu-id="089bf-124">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="089bf-124">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="089bf-125">O operador de comparação de versão do produto.</span><span class="sxs-lookup"><span data-stu-id="089bf-125">The product version comparison operator.</span></span> <span data-ttu-id="089bf-126">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="089bf-126">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="089bf-127">productVersion</span><span class="sxs-lookup"><span data-stu-id="089bf-127">productVersion</span></span>|<span data-ttu-id="089bf-128">String</span><span class="sxs-lookup"><span data-stu-id="089bf-128">String</span></span>|<span data-ttu-id="089bf-129">O valor de comparação da versão do produto.</span><span class="sxs-lookup"><span data-stu-id="089bf-129">The product version comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="089bf-130">Relações</span><span class="sxs-lookup"><span data-stu-id="089bf-130">Relationships</span></span>
<span data-ttu-id="089bf-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="089bf-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="089bf-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="089bf-132">JSON Representation</span></span>
<span data-ttu-id="089bf-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="089bf-133">Here is a JSON representation of the resource.</span></span>
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







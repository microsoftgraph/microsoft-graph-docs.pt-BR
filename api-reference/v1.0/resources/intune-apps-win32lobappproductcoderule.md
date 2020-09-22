---
title: tipo de recurso win32LobAppProductCodeRule
description: Um tipo complexo para armazenar o código do produto e os dados da regra de versão para um aplicativo LOB Win32. Essa regra não é suportada como uma regra de requisito.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 101818fdea0dd87966abdd08d4cfbbffd1a81680
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080036"
---
# <a name="win32lobappproductcoderule-resource-type"></a><span data-ttu-id="71c2a-104">tipo de recurso win32LobAppProductCodeRule</span><span class="sxs-lookup"><span data-stu-id="71c2a-104">win32LobAppProductCodeRule resource type</span></span>

<span data-ttu-id="71c2a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71c2a-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71c2a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71c2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71c2a-107">Um tipo complexo para armazenar o código do produto e os dados da regra de versão para um aplicativo LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="71c2a-107">A complex type to store the product code and version rule data for a Win32 LOB app.</span></span> <span data-ttu-id="71c2a-108">Essa regra não é suportada como uma regra de requisito.</span><span class="sxs-lookup"><span data-stu-id="71c2a-108">This rule is not supported as a requirement rule.</span></span>


<span data-ttu-id="71c2a-109">Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="71c2a-109">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="71c2a-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71c2a-110">Properties</span></span>
|<span data-ttu-id="71c2a-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71c2a-111">Property</span></span>|<span data-ttu-id="71c2a-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="71c2a-112">Type</span></span>|<span data-ttu-id="71c2a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="71c2a-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71c2a-114">ruleType</span><span class="sxs-lookup"><span data-stu-id="71c2a-114">ruleType</span></span>|[<span data-ttu-id="71c2a-115">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="71c2a-115">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="71c2a-116">O tipo de regra que indica o objetivo da regra.</span><span class="sxs-lookup"><span data-stu-id="71c2a-116">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="71c2a-117">Herdado de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="71c2a-117">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="71c2a-118">Os valores possíveis são: `detection` e `requirement`.</span><span class="sxs-lookup"><span data-stu-id="71c2a-118">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="71c2a-119">productCode</span><span class="sxs-lookup"><span data-stu-id="71c2a-119">productCode</span></span>|<span data-ttu-id="71c2a-120">String</span><span class="sxs-lookup"><span data-stu-id="71c2a-120">String</span></span>|<span data-ttu-id="71c2a-121">O código do produto do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="71c2a-121">The product code of the app.</span></span>|
|<span data-ttu-id="71c2a-122">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="71c2a-122">productVersionOperator</span></span>|[<span data-ttu-id="71c2a-123">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="71c2a-123">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="71c2a-124">O operador de comparação de versão do produto.</span><span class="sxs-lookup"><span data-stu-id="71c2a-124">The product version comparison operator.</span></span> <span data-ttu-id="71c2a-125">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="71c2a-125">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="71c2a-126">productVersion</span><span class="sxs-lookup"><span data-stu-id="71c2a-126">productVersion</span></span>|<span data-ttu-id="71c2a-127">String</span><span class="sxs-lookup"><span data-stu-id="71c2a-127">String</span></span>|<span data-ttu-id="71c2a-128">O valor de comparação da versão do produto.</span><span class="sxs-lookup"><span data-stu-id="71c2a-128">The product version comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71c2a-129">Relações</span><span class="sxs-lookup"><span data-stu-id="71c2a-129">Relationships</span></span>
<span data-ttu-id="71c2a-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71c2a-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71c2a-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71c2a-131">JSON Representation</span></span>
<span data-ttu-id="71c2a-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71c2a-132">Here is a JSON representation of the resource.</span></span>
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






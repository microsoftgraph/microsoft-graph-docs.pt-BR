---
title: Tipo de recurso deviceComplianceScriptValidationResult
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d76d96acf8dc96275902d1fba30f8ba6f49cc088
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154275"
---
# <a name="devicecompliancescriptvalidationresult-resource-type"></a><span data-ttu-id="5416e-103">Tipo de recurso deviceComplianceScriptValidationResult</span><span class="sxs-lookup"><span data-stu-id="5416e-103">deviceComplianceScriptValidationResult resource type</span></span>

<span data-ttu-id="5416e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5416e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5416e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5416e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5416e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5416e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5416e-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5416e-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5416e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5416e-108">Properties</span></span>
|<span data-ttu-id="5416e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5416e-109">Property</span></span>|<span data-ttu-id="5416e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5416e-110">Type</span></span>|<span data-ttu-id="5416e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5416e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5416e-112">rules</span><span class="sxs-lookup"><span data-stu-id="5416e-112">rules</span></span>|<span data-ttu-id="5416e-113">[Coleção deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md)</span><span class="sxs-lookup"><span data-stu-id="5416e-113">[deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md) collection</span></span>|<span data-ttu-id="5416e-114">Regras analisados do json.</span><span class="sxs-lookup"><span data-stu-id="5416e-114">Parsed rules from json.</span></span>|
|<span data-ttu-id="5416e-115">scriptErrors</span><span class="sxs-lookup"><span data-stu-id="5416e-115">scriptErrors</span></span>|<span data-ttu-id="5416e-116">[Coleção deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)</span><span class="sxs-lookup"><span data-stu-id="5416e-116">[deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md) collection</span></span>|<span data-ttu-id="5416e-117">Erros em json para o script.</span><span class="sxs-lookup"><span data-stu-id="5416e-117">Errors in json for the script.</span></span>|
|<span data-ttu-id="5416e-118">ruleErrors</span><span class="sxs-lookup"><span data-stu-id="5416e-118">ruleErrors</span></span>|<span data-ttu-id="5416e-119">[Coleção deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md)</span><span class="sxs-lookup"><span data-stu-id="5416e-119">[deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md) collection</span></span>|<span data-ttu-id="5416e-120">Erros em json para o script de regras.</span><span class="sxs-lookup"><span data-stu-id="5416e-120">Errors in json for the script for rules.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5416e-121">Relações</span><span class="sxs-lookup"><span data-stu-id="5416e-121">Relationships</span></span>
<span data-ttu-id="5416e-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5416e-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5416e-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5416e-123">JSON Representation</span></span>
<span data-ttu-id="5416e-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5416e-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptValidationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptValidationResult",
  "rules": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptRule",
      "settingName": "String",
      "operator": "String",
      "deviceComplianceScriptRulOperator": "String",
      "dataType": "String",
      "deviceComplianceScriptRuleDataType": "String",
      "operand": "String"
    }
  ],
  "scriptErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptError",
      "code": "String",
      "deviceComplianceScriptRulesValidationError": "String",
      "message": "String"
    }
  ],
  "ruleErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptRuleError",
      "code": "String",
      "deviceComplianceScriptRulesValidationError": "String",
      "message": "String",
      "settingName": "String"
    }
  ]
}
```





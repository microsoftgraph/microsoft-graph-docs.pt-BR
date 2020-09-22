---
title: tipo de recurso deviceComplianceScriptValidationResult
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8bb60af47f7c06b17dcc54468aa48dd85215a3da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998772"
---
# <a name="devicecompliancescriptvalidationresult-resource-type"></a><span data-ttu-id="accfd-103">tipo de recurso deviceComplianceScriptValidationResult</span><span class="sxs-lookup"><span data-stu-id="accfd-103">deviceComplianceScriptValidationResult resource type</span></span>

<span data-ttu-id="accfd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="accfd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="accfd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="accfd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="accfd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="accfd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="accfd-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="accfd-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="accfd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="accfd-108">Properties</span></span>
|<span data-ttu-id="accfd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="accfd-109">Property</span></span>|<span data-ttu-id="accfd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="accfd-110">Type</span></span>|<span data-ttu-id="accfd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="accfd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="accfd-112">regras</span><span class="sxs-lookup"><span data-stu-id="accfd-112">rules</span></span>|<span data-ttu-id="accfd-113">coleção [deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md)</span><span class="sxs-lookup"><span data-stu-id="accfd-113">[deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md) collection</span></span>|<span data-ttu-id="accfd-114">Regras analisadas do JSON.</span><span class="sxs-lookup"><span data-stu-id="accfd-114">Parsed rules from json.</span></span>|
|<span data-ttu-id="accfd-115">scriptErrors</span><span class="sxs-lookup"><span data-stu-id="accfd-115">scriptErrors</span></span>|<span data-ttu-id="accfd-116">coleção [deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)</span><span class="sxs-lookup"><span data-stu-id="accfd-116">[deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md) collection</span></span>|<span data-ttu-id="accfd-117">Erros no JSON para o script.</span><span class="sxs-lookup"><span data-stu-id="accfd-117">Errors in json for the script.</span></span>|
|<span data-ttu-id="accfd-118">ruleErrors</span><span class="sxs-lookup"><span data-stu-id="accfd-118">ruleErrors</span></span>|<span data-ttu-id="accfd-119">coleção [deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md)</span><span class="sxs-lookup"><span data-stu-id="accfd-119">[deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md) collection</span></span>|<span data-ttu-id="accfd-120">Erros no JSON para o script de regras.</span><span class="sxs-lookup"><span data-stu-id="accfd-120">Errors in json for the script for rules.</span></span>|

## <a name="relationships"></a><span data-ttu-id="accfd-121">Relações</span><span class="sxs-lookup"><span data-stu-id="accfd-121">Relationships</span></span>
<span data-ttu-id="accfd-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="accfd-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="accfd-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="accfd-123">JSON Representation</span></span>
<span data-ttu-id="accfd-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="accfd-124">Here is a JSON representation of the resource.</span></span>
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
      "dataType": "String",
      "operand": "String"
    }
  ],
  "scriptErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptError",
      "code": "String",
      "message": "String"
    }
  ],
  "ruleErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptRuleError",
      "code": "String",
      "message": "String",
      "settingName": "String"
    }
  ]
}
```







---
title: tipo de recurso deviceComplianceScriptValidationResult
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6670b5eeb4dbdfc37535d930677550a685cb405c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260205"
---
# <a name="devicecompliancescriptvalidationresult-resource-type"></a><span data-ttu-id="3f246-103">tipo de recurso deviceComplianceScriptValidationResult</span><span class="sxs-lookup"><span data-stu-id="3f246-103">deviceComplianceScriptValidationResult resource type</span></span>

<span data-ttu-id="3f246-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f246-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f246-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3f246-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f246-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3f246-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f246-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3f246-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3f246-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f246-108">Properties</span></span>
|<span data-ttu-id="3f246-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f246-109">Property</span></span>|<span data-ttu-id="3f246-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f246-110">Type</span></span>|<span data-ttu-id="3f246-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f246-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f246-112">regras</span><span class="sxs-lookup"><span data-stu-id="3f246-112">rules</span></span>|<span data-ttu-id="3f246-113">coleção [deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md)</span><span class="sxs-lookup"><span data-stu-id="3f246-113">[deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md) collection</span></span>|<span data-ttu-id="3f246-114">Regras analisadas do JSON.</span><span class="sxs-lookup"><span data-stu-id="3f246-114">Parsed rules from json.</span></span>|
|<span data-ttu-id="3f246-115">scriptErrors</span><span class="sxs-lookup"><span data-stu-id="3f246-115">scriptErrors</span></span>|<span data-ttu-id="3f246-116">coleção [deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)</span><span class="sxs-lookup"><span data-stu-id="3f246-116">[deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md) collection</span></span>|<span data-ttu-id="3f246-117">Erros no JSON para o script.</span><span class="sxs-lookup"><span data-stu-id="3f246-117">Errors in json for the script.</span></span>|
|<span data-ttu-id="3f246-118">ruleErrors</span><span class="sxs-lookup"><span data-stu-id="3f246-118">ruleErrors</span></span>|<span data-ttu-id="3f246-119">coleção [deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md)</span><span class="sxs-lookup"><span data-stu-id="3f246-119">[deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md) collection</span></span>|<span data-ttu-id="3f246-120">Erros no JSON para o script de regras.</span><span class="sxs-lookup"><span data-stu-id="3f246-120">Errors in json for the script for rules.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f246-121">Relações</span><span class="sxs-lookup"><span data-stu-id="3f246-121">Relationships</span></span>
<span data-ttu-id="3f246-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f246-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f246-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f246-123">JSON Representation</span></span>
<span data-ttu-id="3f246-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f246-124">Here is a JSON representation of the resource.</span></span>
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





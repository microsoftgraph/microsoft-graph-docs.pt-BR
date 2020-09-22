---
title: tipo de recurso deviceComplianceScriptError
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c0ea8bf7c882d7a31c4f4477c7d7b74994676497
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026779"
---
# <a name="devicecompliancescripterror-resource-type"></a><span data-ttu-id="740fe-103">tipo de recurso deviceComplianceScriptError</span><span class="sxs-lookup"><span data-stu-id="740fe-103">deviceComplianceScriptError resource type</span></span>

<span data-ttu-id="740fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="740fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="740fe-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="740fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="740fe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="740fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="740fe-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="740fe-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="740fe-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="740fe-108">Properties</span></span>
|<span data-ttu-id="740fe-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="740fe-109">Property</span></span>|<span data-ttu-id="740fe-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="740fe-110">Type</span></span>|<span data-ttu-id="740fe-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="740fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="740fe-112">código</span><span class="sxs-lookup"><span data-stu-id="740fe-112">code</span></span>|[<span data-ttu-id="740fe-113">code</span><span class="sxs-lookup"><span data-stu-id="740fe-113">code</span></span>](../resources/intune-deviceconfig-code.md)|<span data-ttu-id="740fe-114">Código de erro.</span><span class="sxs-lookup"><span data-stu-id="740fe-114">Error code.</span></span> <span data-ttu-id="740fe-115">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, `none` `jsonFileInvalid` `jsonFileMissing` `jsonFileTooLarge` `rulesMissing` `duplicateRules` `tooManyRulesSpecified` `operatorMissing` `operatorNotSupported` `datatypeMissing` `datatypeNotSupported` `operatorDataTypeCombinationNotSupported` `moreInfoUriMissing` `moreInfoUriInvalid` `moreInfoUriTooLarge` `descriptionMissing` `descriptionInvalid` `descriptionTooLarge` `titleMissing` `titleInvalid` `titleTooLarge` `operandMissing` `operandInvalid` `operandTooLarge` `settingNameMissing` `settingNameInvalid` `settingNameTooLarge` `englishLocaleMissing` `duplicateLocales` `unrecognizedLocale` `unknown` `remediationStringsMissing` .</span><span class="sxs-lookup"><span data-stu-id="740fe-115">Possible values are: `none`, `jsonFileInvalid`, `jsonFileMissing`, `jsonFileTooLarge`, `rulesMissing`, `duplicateRules`, `tooManyRulesSpecified`, `operatorMissing`, `operatorNotSupported`, `datatypeMissing`, `datatypeNotSupported`, `operatorDataTypeCombinationNotSupported`, `moreInfoUriMissing`, `moreInfoUriInvalid`, `moreInfoUriTooLarge`, `descriptionMissing`, `descriptionInvalid`, `descriptionTooLarge`, `titleMissing`, `titleInvalid`, `titleTooLarge`, `operandMissing`, `operandInvalid`, `operandTooLarge`, `settingNameMissing`, `settingNameInvalid`, `settingNameTooLarge`, `englishLocaleMissing`, `duplicateLocales`, `unrecognizedLocale`, `unknown`, `remediationStringsMissing`.</span></span>|
|<span data-ttu-id="740fe-116">mensagem</span><span class="sxs-lookup"><span data-stu-id="740fe-116">message</span></span>|<span data-ttu-id="740fe-117">String</span><span class="sxs-lookup"><span data-stu-id="740fe-117">String</span></span>|<span data-ttu-id="740fe-118">Mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="740fe-118">Error message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="740fe-119">Relações</span><span class="sxs-lookup"><span data-stu-id="740fe-119">Relationships</span></span>
<span data-ttu-id="740fe-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="740fe-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="740fe-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="740fe-121">JSON Representation</span></span>
<span data-ttu-id="740fe-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="740fe-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptError",
  "code": "String",
  "message": "String"
}
```







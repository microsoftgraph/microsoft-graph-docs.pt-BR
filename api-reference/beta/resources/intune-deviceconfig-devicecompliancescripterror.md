---
title: tipo de recurso deviceComplianceScriptError
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd8a801d34bb5a7ad07c7e769d25fa0a05e31a53
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260254"
---
# <a name="devicecompliancescripterror-resource-type"></a><span data-ttu-id="49039-103">tipo de recurso deviceComplianceScriptError</span><span class="sxs-lookup"><span data-stu-id="49039-103">deviceComplianceScriptError resource type</span></span>

<span data-ttu-id="49039-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49039-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49039-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49039-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49039-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49039-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49039-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="49039-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="49039-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49039-108">Properties</span></span>
|<span data-ttu-id="49039-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49039-109">Property</span></span>|<span data-ttu-id="49039-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="49039-110">Type</span></span>|<span data-ttu-id="49039-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="49039-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49039-112">código</span><span class="sxs-lookup"><span data-stu-id="49039-112">code</span></span>|[<span data-ttu-id="49039-113">code</span><span class="sxs-lookup"><span data-stu-id="49039-113">code</span></span>](../resources/intune-deviceconfig-code.md)|<span data-ttu-id="49039-114">Código de erro.</span><span class="sxs-lookup"><span data-stu-id="49039-114">Error code.</span></span> <span data-ttu-id="49039-115">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, `none` `jsonFileInvalid` `jsonFileMissing` `jsonFileTooLarge` `rulesMissing` `duplicateRules` `tooManyRulesSpecified` `operatorMissing` `operatorNotSupported` `datatypeMissing` `datatypeNotSupported` `operatorDataTypeCombinationNotSupported` `moreInfoUriMissing` `moreInfoUriInvalid` `moreInfoUriTooLarge` `descriptionMissing` `descriptionInvalid` `descriptionTooLarge` `titleMissing` `titleInvalid` `titleTooLarge` `operandMissing` `operandInvalid` `operandTooLarge` `settingNameMissing` `settingNameInvalid` `settingNameTooLarge` `englishLocaleMissing` `duplicateLocales` `unrecognizedLocale` `unknown` `remediationStringsMissing` .</span><span class="sxs-lookup"><span data-stu-id="49039-115">Possible values are: `none`, `jsonFileInvalid`, `jsonFileMissing`, `jsonFileTooLarge`, `rulesMissing`, `duplicateRules`, `tooManyRulesSpecified`, `operatorMissing`, `operatorNotSupported`, `datatypeMissing`, `datatypeNotSupported`, `operatorDataTypeCombinationNotSupported`, `moreInfoUriMissing`, `moreInfoUriInvalid`, `moreInfoUriTooLarge`, `descriptionMissing`, `descriptionInvalid`, `descriptionTooLarge`, `titleMissing`, `titleInvalid`, `titleTooLarge`, `operandMissing`, `operandInvalid`, `operandTooLarge`, `settingNameMissing`, `settingNameInvalid`, `settingNameTooLarge`, `englishLocaleMissing`, `duplicateLocales`, `unrecognizedLocale`, `unknown`, `remediationStringsMissing`.</span></span>|
|<span data-ttu-id="49039-116">mensagem</span><span class="sxs-lookup"><span data-stu-id="49039-116">message</span></span>|<span data-ttu-id="49039-117">String</span><span class="sxs-lookup"><span data-stu-id="49039-117">String</span></span>|<span data-ttu-id="49039-118">Mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="49039-118">Error message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49039-119">Relações</span><span class="sxs-lookup"><span data-stu-id="49039-119">Relationships</span></span>
<span data-ttu-id="49039-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="49039-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49039-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49039-121">JSON Representation</span></span>
<span data-ttu-id="49039-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="49039-122">Here is a JSON representation of the resource.</span></span>
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





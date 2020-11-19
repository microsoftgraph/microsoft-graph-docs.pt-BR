---
title: tipo de recurso deviceManagementConfigurationStringSettingValueDefinition
description: Restrições de cadeia de caracteres
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03a96252cffabddd2acb613ff365fd16951fd55c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241242"
---
# <a name="devicemanagementconfigurationstringsettingvaluedefinition-resource-type"></a><span data-ttu-id="44820-103">tipo de recurso deviceManagementConfigurationStringSettingValueDefinition</span><span class="sxs-lookup"><span data-stu-id="44820-103">deviceManagementConfigurationStringSettingValueDefinition resource type</span></span>

<span data-ttu-id="44820-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44820-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44820-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="44820-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44820-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44820-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44820-107">Restrições de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44820-107">String constraints</span></span>


<span data-ttu-id="44820-108">Herda de [deviceManagementConfigurationSettingValueDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)</span><span class="sxs-lookup"><span data-stu-id="44820-108">Inherits from [deviceManagementConfigurationSettingValueDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)</span></span>

## <a name="properties"></a><span data-ttu-id="44820-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44820-109">Properties</span></span>
|<span data-ttu-id="44820-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44820-110">Property</span></span>|<span data-ttu-id="44820-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="44820-111">Type</span></span>|<span data-ttu-id="44820-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="44820-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44820-113">formato</span><span class="sxs-lookup"><span data-stu-id="44820-113">format</span></span>|[<span data-ttu-id="44820-114">deviceManagementConfigurationStringFormat</span><span class="sxs-lookup"><span data-stu-id="44820-114">deviceManagementConfigurationStringFormat</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringformat.md)|<span data-ttu-id="44820-115">Formato predefinido da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="44820-115">Pre-defined format of the string.</span></span> <span data-ttu-id="44820-116">Os valores possíveis são:, `none` `email` , `guid` , `ip` , `base64` , `url` , `version` , `xml` , `date` , `time` , `binary` , `regEx` ,, `json` `dateTime` `surfaceHub` .</span><span class="sxs-lookup"><span data-stu-id="44820-116">Possible values are: `none`, `email`, `guid`, `ip`, `base64`, `url`, `version`, `xml`, `date`, `time`, `binary`, `regEx`, `json`, `dateTime`, `surfaceHub`.</span></span>|
|<span data-ttu-id="44820-117">inputValidationSchema</span><span class="sxs-lookup"><span data-stu-id="44820-117">inputValidationSchema</span></span>|<span data-ttu-id="44820-118">String</span><span class="sxs-lookup"><span data-stu-id="44820-118">String</span></span>|<span data-ttu-id="44820-119">Expressão regular ou qualquer esquema XML ou JSON que a cadeia de caracteres de entrada deve corresponder</span><span class="sxs-lookup"><span data-stu-id="44820-119">Regular expression or any xml or json schema that the input string should match</span></span>|
|<span data-ttu-id="44820-120">maximumLength</span><span class="sxs-lookup"><span data-stu-id="44820-120">maximumLength</span></span>|<span data-ttu-id="44820-121">Int64</span><span class="sxs-lookup"><span data-stu-id="44820-121">Int64</span></span>|<span data-ttu-id="44820-122">Comprimento máximo da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="44820-122">Maximum length of string.</span></span> <span data-ttu-id="44820-123">Valores válidos de 0 a 87516</span><span class="sxs-lookup"><span data-stu-id="44820-123">Valid values 0 to 87516</span></span>|
|<span data-ttu-id="44820-124">minimumLength</span><span class="sxs-lookup"><span data-stu-id="44820-124">minimumLength</span></span>|<span data-ttu-id="44820-125">Int64</span><span class="sxs-lookup"><span data-stu-id="44820-125">Int64</span></span>|<span data-ttu-id="44820-126">Comprimento mínimo da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="44820-126">Minimum length of string.</span></span> <span data-ttu-id="44820-127">Valores válidos de 0 a 87516</span><span class="sxs-lookup"><span data-stu-id="44820-127">Valid values 0 to 87516</span></span>|
|<span data-ttu-id="44820-128">issecret</span><span class="sxs-lookup"><span data-stu-id="44820-128">isSecret</span></span>|<span data-ttu-id="44820-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="44820-129">Boolean</span></span>|<span data-ttu-id="44820-130">Especifica se a configuração deve ser tratada como um segredo.</span><span class="sxs-lookup"><span data-stu-id="44820-130">Specifies whether the setting needs to be treated as a secret.</span></span> <span data-ttu-id="44820-131">As configurações marcadas como Sim serão criptografadas em trânsito e em repouso e serão exibidas como asteriscos quando forem representadas no UX.</span><span class="sxs-lookup"><span data-stu-id="44820-131">Settings marked as yes will be encrypted in transit and at rest and will be displayed as asterisks when represented in the UX.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44820-132">Relações</span><span class="sxs-lookup"><span data-stu-id="44820-132">Relationships</span></span>
<span data-ttu-id="44820-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="44820-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44820-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44820-134">JSON Representation</span></span>
<span data-ttu-id="44820-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="44820-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationStringSettingValueDefinition",
  "format": "String",
  "inputValidationSchema": "String",
  "maximumLength": 1024,
  "minimumLength": 1024,
  "isSecret": true
}
```





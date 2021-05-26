---
title: Tipo de recurso deviceManagementConfigurationIntegerSettingValueTemplate
description: Modelo de valor de configuração de inteiro
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1a196cf31bbb1a7063b6d937e797d602e7481ff4
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666780"
---
# <a name="devicemanagementconfigurationintegersettingvaluetemplate-resource-type"></a><span data-ttu-id="59240-103">Tipo de recurso deviceManagementConfigurationIntegerSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="59240-103">deviceManagementConfigurationIntegerSettingValueTemplate resource type</span></span>

<span data-ttu-id="59240-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59240-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59240-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="59240-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59240-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59240-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59240-107">Modelo de valor de configuração de inteiro</span><span class="sxs-lookup"><span data-stu-id="59240-107">Integer Setting Value Template</span></span>


<span data-ttu-id="59240-108">Herda [de deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="59240-108">Inherits from [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="59240-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59240-109">Properties</span></span>
|<span data-ttu-id="59240-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59240-110">Property</span></span>|<span data-ttu-id="59240-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="59240-111">Type</span></span>|<span data-ttu-id="59240-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="59240-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59240-113">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="59240-113">settingValueTemplateId</span></span>|<span data-ttu-id="59240-114">String</span><span class="sxs-lookup"><span data-stu-id="59240-114">String</span></span>|<span data-ttu-id="59240-115">Definição da ID do Modelo de Valor Herdada [de deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="59240-115">Setting Value Template Id Inherited from [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span></span>|
|<span data-ttu-id="59240-116">defaultValue</span><span class="sxs-lookup"><span data-stu-id="59240-116">defaultValue</span></span>|[<span data-ttu-id="59240-117">deviceManagementConfigurationIntegerSettingValueDefaultTemplate</span><span class="sxs-lookup"><span data-stu-id="59240-117">deviceManagementConfigurationIntegerSettingValueDefaultTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefaulttemplate.md)|<span data-ttu-id="59240-118">Modelo padrão de valor de configuração de inteiro.</span><span class="sxs-lookup"><span data-stu-id="59240-118">Integer Setting Value Default Template.</span></span>|
|<span data-ttu-id="59240-119">recommendedValueDefinition</span><span class="sxs-lookup"><span data-stu-id="59240-119">recommendedValueDefinition</span></span>|[<span data-ttu-id="59240-120">deviceManagementConfigurationIntegerSettingValueDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="59240-120">deviceManagementConfigurationIntegerSettingValueDefinitionTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefinitiontemplate.md)|<span data-ttu-id="59240-121">Definição de valor recomendada.</span><span class="sxs-lookup"><span data-stu-id="59240-121">Recommended value definition.</span></span>|
|<span data-ttu-id="59240-122">requiredValueDefinition</span><span class="sxs-lookup"><span data-stu-id="59240-122">requiredValueDefinition</span></span>|[<span data-ttu-id="59240-123">deviceManagementConfigurationIntegerSettingValueDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="59240-123">deviceManagementConfigurationIntegerSettingValueDefinitionTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefinitiontemplate.md)|<span data-ttu-id="59240-124">Definição de valor necessária.</span><span class="sxs-lookup"><span data-stu-id="59240-124">Required value definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59240-125">Relações</span><span class="sxs-lookup"><span data-stu-id="59240-125">Relationships</span></span>
<span data-ttu-id="59240-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="59240-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59240-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59240-127">JSON Representation</span></span>
<span data-ttu-id="59240-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="59240-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValueTemplate",
  "settingValueTemplateId": "String",
  "defaultValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate",
    "constantValue": 1024
  },
  "recommendedValueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate",
    "minValue": 1024,
    "maxValue": 1024
  },
  "requiredValueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate",
    "minValue": 1024,
    "maxValue": 1024
  }
}
```





---
title: Tipo de recurso deviceManagementConfigurationGroupSettingInstanceTemplate
description: Modelo de Instância de Configuração de Grupo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 71536897dd8a214e0e4b1c794b7329a3b004afbf
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666545"
---
# <a name="devicemanagementconfigurationgroupsettinginstancetemplate-resource-type"></a><span data-ttu-id="89591-103">Tipo de recurso deviceManagementConfigurationGroupSettingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="89591-103">deviceManagementConfigurationGroupSettingInstanceTemplate resource type</span></span>

<span data-ttu-id="89591-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89591-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89591-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="89591-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89591-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89591-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89591-107">Modelo de Instância de Configuração de Grupo</span><span class="sxs-lookup"><span data-stu-id="89591-107">Group Setting Instance Template</span></span>


<span data-ttu-id="89591-108">Herda de [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="89591-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="89591-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89591-109">Properties</span></span>
|<span data-ttu-id="89591-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89591-110">Property</span></span>|<span data-ttu-id="89591-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="89591-111">Type</span></span>|<span data-ttu-id="89591-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="89591-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89591-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="89591-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="89591-114">String</span><span class="sxs-lookup"><span data-stu-id="89591-114">String</span></span>|<span data-ttu-id="89591-115">Id do modelo de instância de configuração Herdada [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="89591-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="89591-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="89591-116">settingDefinitionId</span></span>|<span data-ttu-id="89591-117">String</span><span class="sxs-lookup"><span data-stu-id="89591-117">String</span></span>|<span data-ttu-id="89591-118">Definição Id De definição Herdada [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="89591-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="89591-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="89591-119">isRequired</span></span>|<span data-ttu-id="89591-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="89591-120">Boolean</span></span>|<span data-ttu-id="89591-121">Indica se uma política deve especificar essa configuração.</span><span class="sxs-lookup"><span data-stu-id="89591-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="89591-122">Herdado [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="89591-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="89591-123">groupSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="89591-123">groupSettingValueTemplate</span></span>|[<span data-ttu-id="89591-124">deviceManagementConfigurationGroupSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="89591-124">deviceManagementConfigurationGroupSettingValueTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvaluetemplate.md)|<span data-ttu-id="89591-125">Modelo de valor de configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="89591-125">Group Setting Value Template</span></span>|

## <a name="relationships"></a><span data-ttu-id="89591-126">Relações</span><span class="sxs-lookup"><span data-stu-id="89591-126">Relationships</span></span>
<span data-ttu-id="89591-127">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="89591-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89591-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89591-128">JSON Representation</span></span>
<span data-ttu-id="89591-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89591-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationGroupSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "groupSettingValueTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValueTemplate",
    "children": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
        "settingInstanceTemplateId": "String",
        "settingDefinitionId": "String",
        "isRequired": true,
        "simpleSettingValueTemplate": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
          "settingValueTemplateId": "String",
          "defaultValue": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
            "constantValue": "String"
          }
        }
      }
    ],
    "settingValueTemplateId": "String"
  }
}
```





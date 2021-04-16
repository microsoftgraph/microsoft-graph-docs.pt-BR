---
title: Tipo de recurso deviceManagementConfigurationChoiceSettingInstanceTemplate
description: Modelo de instância de configuração de opção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b7c894e455d96f1fb7e8c2cd7a50beaff009858f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868317"
---
# <a name="devicemanagementconfigurationchoicesettinginstancetemplate-resource-type"></a><span data-ttu-id="84ff2-103">Tipo de recurso deviceManagementConfigurationChoiceSettingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="84ff2-103">deviceManagementConfigurationChoiceSettingInstanceTemplate resource type</span></span>

<span data-ttu-id="84ff2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84ff2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84ff2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="84ff2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84ff2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84ff2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84ff2-107">Modelo de instância de configuração de opção</span><span class="sxs-lookup"><span data-stu-id="84ff2-107">Choice Setting Instance Template</span></span>


<span data-ttu-id="84ff2-108">Herda de [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="84ff2-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="84ff2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84ff2-109">Properties</span></span>
|<span data-ttu-id="84ff2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84ff2-110">Property</span></span>|<span data-ttu-id="84ff2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="84ff2-111">Type</span></span>|<span data-ttu-id="84ff2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="84ff2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84ff2-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="84ff2-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="84ff2-114">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="84ff2-114">String</span></span>|<span data-ttu-id="84ff2-115">Id do modelo de instância de configuração Herdada [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="84ff2-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="84ff2-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="84ff2-116">settingDefinitionId</span></span>|<span data-ttu-id="84ff2-117">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="84ff2-117">String</span></span>|<span data-ttu-id="84ff2-118">Definição Id De definição Herdada [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="84ff2-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="84ff2-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="84ff2-119">isRequired</span></span>|<span data-ttu-id="84ff2-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="84ff2-120">Boolean</span></span>|<span data-ttu-id="84ff2-121">Indica se uma política deve especificar essa configuração.</span><span class="sxs-lookup"><span data-stu-id="84ff2-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="84ff2-122">Herdado [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="84ff2-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="84ff2-123">choiceSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="84ff2-123">choiceSettingValueTemplate</span></span>|[<span data-ttu-id="84ff2-124">deviceManagementConfigurationChoiceSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="84ff2-124">deviceManagementConfigurationChoiceSettingValueTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluetemplate.md)|<span data-ttu-id="84ff2-125">Modelo de valor de configuração de opção</span><span class="sxs-lookup"><span data-stu-id="84ff2-125">Choice Setting Value Template</span></span>|

## <a name="relationships"></a><span data-ttu-id="84ff2-126">Relações</span><span class="sxs-lookup"><span data-stu-id="84ff2-126">Relationships</span></span>
<span data-ttu-id="84ff2-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="84ff2-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84ff2-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84ff2-128">JSON Representation</span></span>
<span data-ttu-id="84ff2-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84ff2-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "choiceSettingValueTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueTemplate",
    "defaultValue": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate",
      "settingDefinitionOptionId": "String",
      "children": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
          "settingInstanceTemplateId": "String",
          "settingDefinitionId": "String",
          "isRequired": true,
          "simpleSettingValueTemplate": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
            "settingValueTemplateId": "String"
          }
        }
      ]
    },
    "recommendedValueDefinition": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
      "allowedOptions": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
          "itemId": "String",
          "children": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
              "settingInstanceTemplateId": "String",
              "settingDefinitionId": "String",
              "isRequired": true,
              "simpleSettingValueTemplate": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
                "settingValueTemplateId": "String"
              }
            }
          ]
        }
      ]
    },
    "requiredValueDefinition": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
      "allowedOptions": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
          "itemId": "String",
          "children": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
              "settingInstanceTemplateId": "String",
              "settingDefinitionId": "String",
              "isRequired": true,
              "simpleSettingValueTemplate": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
                "settingValueTemplateId": "String"
              }
            }
          ]
        }
      ]
    },
    "settingValueTemplateId": "String"
  }
}
```





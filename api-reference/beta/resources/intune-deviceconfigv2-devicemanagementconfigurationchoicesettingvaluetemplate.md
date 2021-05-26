---
title: Tipo de recurso deviceManagementConfigurationChoiceSettingValueTemplate
description: Modelo de valor de configuração de opção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 10d446532e0664c6d83d16d223c0a8e0d966aeb4
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666573"
---
# <a name="devicemanagementconfigurationchoicesettingvaluetemplate-resource-type"></a><span data-ttu-id="71b8a-103">Tipo de recurso deviceManagementConfigurationChoiceSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="71b8a-103">deviceManagementConfigurationChoiceSettingValueTemplate resource type</span></span>

<span data-ttu-id="71b8a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71b8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71b8a-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71b8a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71b8a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71b8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71b8a-107">Modelo de valor de configuração de opção</span><span class="sxs-lookup"><span data-stu-id="71b8a-107">Choice Setting Value Template</span></span>

## <a name="properties"></a><span data-ttu-id="71b8a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71b8a-108">Properties</span></span>
|<span data-ttu-id="71b8a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71b8a-109">Property</span></span>|<span data-ttu-id="71b8a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="71b8a-110">Type</span></span>|<span data-ttu-id="71b8a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="71b8a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71b8a-112">defaultValue</span><span class="sxs-lookup"><span data-stu-id="71b8a-112">defaultValue</span></span>|[<span data-ttu-id="71b8a-113">deviceManagementConfigurationChoiceSettingValueDefaultTemplate</span><span class="sxs-lookup"><span data-stu-id="71b8a-113">deviceManagementConfigurationChoiceSettingValueDefaultTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefaulttemplate.md)|<span data-ttu-id="71b8a-114">Modelo padrão de valor de configuração de opção.</span><span class="sxs-lookup"><span data-stu-id="71b8a-114">Choice Setting Value Default Template.</span></span>|
|<span data-ttu-id="71b8a-115">recommendedValueDefinition</span><span class="sxs-lookup"><span data-stu-id="71b8a-115">recommendedValueDefinition</span></span>|[<span data-ttu-id="71b8a-116">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="71b8a-116">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefinitiontemplate.md)|<span data-ttu-id="71b8a-117">Substituição de definição recomendada.</span><span class="sxs-lookup"><span data-stu-id="71b8a-117">Recommended definition override.</span></span>|
|<span data-ttu-id="71b8a-118">requiredValueDefinition</span><span class="sxs-lookup"><span data-stu-id="71b8a-118">requiredValueDefinition</span></span>|[<span data-ttu-id="71b8a-119">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="71b8a-119">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefinitiontemplate.md)|<span data-ttu-id="71b8a-120">Substituição de definição necessária.</span><span class="sxs-lookup"><span data-stu-id="71b8a-120">Required definition override.</span></span>|
|<span data-ttu-id="71b8a-121">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="71b8a-121">settingValueTemplateId</span></span>|<span data-ttu-id="71b8a-122">String</span><span class="sxs-lookup"><span data-stu-id="71b8a-122">String</span></span>|<span data-ttu-id="71b8a-123">Definindo a ID do Modelo de Valor</span><span class="sxs-lookup"><span data-stu-id="71b8a-123">Setting Value Template Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="71b8a-124">Relações</span><span class="sxs-lookup"><span data-stu-id="71b8a-124">Relationships</span></span>
<span data-ttu-id="71b8a-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="71b8a-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71b8a-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71b8a-126">JSON Representation</span></span>
<span data-ttu-id="71b8a-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71b8a-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValueTemplate",
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
          "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
          "settingValueTemplateId": "String",
          "defaultValue": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
            "constantValue": "String"
          }
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
              "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
              "settingValueTemplateId": "String",
              "defaultValue": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
                "constantValue": "String"
              }
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
              "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
              "settingValueTemplateId": "String",
              "defaultValue": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
                "constantValue": "String"
              }
            }
          }
        ]
      }
    ]
  },
  "settingValueTemplateId": "String"
}
```





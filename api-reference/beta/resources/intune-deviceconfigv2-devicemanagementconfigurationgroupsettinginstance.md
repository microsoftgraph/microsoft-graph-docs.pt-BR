---
title: tipo de recurso deviceManagementConfigurationGroupSettingInstance
description: Instância de um GroupSetting
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb5105acb3e975811400bd9784803c97db0c5370
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241174"
---
# <a name="devicemanagementconfigurationgroupsettinginstance-resource-type"></a><span data-ttu-id="a83c4-103">tipo de recurso deviceManagementConfigurationGroupSettingInstance</span><span class="sxs-lookup"><span data-stu-id="a83c4-103">deviceManagementConfigurationGroupSettingInstance resource type</span></span>

<span data-ttu-id="a83c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a83c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a83c4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a83c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a83c4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a83c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a83c4-107">Instância de um GroupSetting</span><span class="sxs-lookup"><span data-stu-id="a83c4-107">Instance of a GroupSetting</span></span>


<span data-ttu-id="a83c4-108">Herda de [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="a83c4-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a83c4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a83c4-109">Properties</span></span>
|<span data-ttu-id="a83c4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a83c4-110">Property</span></span>|<span data-ttu-id="a83c4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a83c4-111">Type</span></span>|<span data-ttu-id="a83c4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a83c4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a83c4-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a83c4-113">settingDefinitionId</span></span>|<span data-ttu-id="a83c4-114">String</span><span class="sxs-lookup"><span data-stu-id="a83c4-114">String</span></span>|<span data-ttu-id="a83c4-115">Definição de ID de definição herdada de [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="a83c4-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="a83c4-116">groupSettingValue</span><span class="sxs-lookup"><span data-stu-id="a83c4-116">groupSettingValue</span></span>|[<span data-ttu-id="a83c4-117">deviceManagementConfigurationGroupSettingValue</span><span class="sxs-lookup"><span data-stu-id="a83c4-117">deviceManagementConfigurationGroupSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvalue.md)|<span data-ttu-id="a83c4-118">Valor GroupSetting</span><span class="sxs-lookup"><span data-stu-id="a83c4-118">GroupSetting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="a83c4-119">Relações</span><span class="sxs-lookup"><span data-stu-id="a83c4-119">Relationships</span></span>
<span data-ttu-id="a83c4-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a83c4-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a83c4-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a83c4-121">JSON Representation</span></span>
<span data-ttu-id="a83c4-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a83c4-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationGroupSettingInstance",
  "settingDefinitionId": "String",
  "groupSettingValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValue",
    "children": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
        "settingDefinitionId": "String",
        "choiceSettingValue": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
          "value": "String",
          "children": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
              "settingDefinitionId": "String",
              "choiceSettingValue": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                "value": "String",
                "children": [
                  {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                    "settingDefinitionId": "String",
                    "choiceSettingValue": {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                      "value": "String",
                      "children": [
                        {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                          "settingDefinitionId": "String",
                          "choiceSettingValue": {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                            "value": "String",
                            "children": [
                              {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                "settingDefinitionId": "String",
                                "choiceSettingValue": {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                  "value": "String",
                                  "children": [
                                    {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                      "settingDefinitionId": "String",
                                      "choiceSettingValue": {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                        "value": "String",
                                        "children": [
                                          {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                            "settingDefinitionId": "String",
                                            "choiceSettingValue": {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                              "value": "String",
                                              "children": [
                                                {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                  "settingDefinitionId": "String",
                                                  "choiceSettingValue": {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                    "value": "String",
                                                    "children": [
                                                      {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                        "settingDefinitionId": "String",
                                                        "choiceSettingValue": {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                          "value": "String",
                                                          "children": [
                                                            {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                              "settingDefinitionId": "String",
                                                              "choiceSettingValue": {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                "value": "String",
                                                                "children": [
                                                                  {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                    "settingDefinitionId": "String",
                                                                    "choiceSettingValue": {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                      "value": "String",
                                                                      "children": null
                                                                    }
                                                                  }
                                                                ]
                                                              }
                                                            }
                                                          ]
                                                        }
                                                      }
                                                    ]
                                                  }
                                                }
                                              ]
                                            }
                                          }
                                        ]
                                      }
                                    }
                                  ]
                                }
                              }
                            ]
                          }
                        }
                      ]
                    }
                  }
                ]
              }
            }
          ]
        }
      }
    ]
  }
}
```





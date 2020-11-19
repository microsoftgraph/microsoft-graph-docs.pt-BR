---
title: tipo de recurso deviceManagementConfigurationGroupSettingCollectionInstance
description: Instância de um GroupSettingCollection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 40542c7358838f60bfeb30d8e938062fbbc2c7b0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241175"
---
# <a name="devicemanagementconfigurationgroupsettingcollectioninstance-resource-type"></a><span data-ttu-id="b00c0-103">tipo de recurso deviceManagementConfigurationGroupSettingCollectionInstance</span><span class="sxs-lookup"><span data-stu-id="b00c0-103">deviceManagementConfigurationGroupSettingCollectionInstance resource type</span></span>

<span data-ttu-id="b00c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b00c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b00c0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b00c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b00c0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b00c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b00c0-107">Instância de um GroupSettingCollection</span><span class="sxs-lookup"><span data-stu-id="b00c0-107">Instance of a GroupSettingCollection</span></span>


<span data-ttu-id="b00c0-108">Herda de [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="b00c0-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b00c0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b00c0-109">Properties</span></span>
|<span data-ttu-id="b00c0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b00c0-110">Property</span></span>|<span data-ttu-id="b00c0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b00c0-111">Type</span></span>|<span data-ttu-id="b00c0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b00c0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b00c0-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b00c0-113">settingDefinitionId</span></span>|<span data-ttu-id="b00c0-114">String</span><span class="sxs-lookup"><span data-stu-id="b00c0-114">String</span></span>|<span data-ttu-id="b00c0-115">Definição de ID de definição herdada de [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="b00c0-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="b00c0-116">groupSettingCollectionValue</span><span class="sxs-lookup"><span data-stu-id="b00c0-116">groupSettingCollectionValue</span></span>|<span data-ttu-id="b00c0-117">coleção [deviceManagementConfigurationGroupSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b00c0-117">[deviceManagementConfigurationGroupSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvalue.md) collection</span></span>|<span data-ttu-id="b00c0-118">Uma coleção de valores GroupSetting</span><span class="sxs-lookup"><span data-stu-id="b00c0-118">A collection of GroupSetting values</span></span>|

## <a name="relationships"></a><span data-ttu-id="b00c0-119">Relações</span><span class="sxs-lookup"><span data-stu-id="b00c0-119">Relationships</span></span>
<span data-ttu-id="b00c0-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b00c0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b00c0-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b00c0-121">JSON Representation</span></span>
<span data-ttu-id="b00c0-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b00c0-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationGroupSettingCollectionInstance",
  "settingDefinitionId": "String",
  "groupSettingCollectionValue": [
    {
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
  ]
}
```





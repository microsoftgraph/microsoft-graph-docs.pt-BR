---
title: tipo de recurso deviceManagementConfigurationChoiceSettingValue
description: Valor de configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d7b57e1cb62feb48073207275c249796a2474294
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241180"
---
# <a name="devicemanagementconfigurationchoicesettingvalue-resource-type"></a><span data-ttu-id="27391-103">tipo de recurso deviceManagementConfigurationChoiceSettingValue</span><span class="sxs-lookup"><span data-stu-id="27391-103">deviceManagementConfigurationChoiceSettingValue resource type</span></span>

<span data-ttu-id="27391-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27391-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27391-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="27391-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27391-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27391-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27391-107">Valor de configuração</span><span class="sxs-lookup"><span data-stu-id="27391-107">Setting value</span></span>


<span data-ttu-id="27391-108">Herda de [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="27391-108">Inherits from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="27391-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27391-109">Properties</span></span>
|<span data-ttu-id="27391-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27391-110">Property</span></span>|<span data-ttu-id="27391-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="27391-111">Type</span></span>|<span data-ttu-id="27391-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="27391-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27391-113">valor</span><span class="sxs-lookup"><span data-stu-id="27391-113">value</span></span>|<span data-ttu-id="27391-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27391-114">String</span></span>|<span data-ttu-id="27391-115">Valor de configuração de opção: uma ItemId OptionDefinition.</span><span class="sxs-lookup"><span data-stu-id="27391-115">Choice setting value: an OptionDefinition ItemId.</span></span>|
|<span data-ttu-id="27391-116">children</span><span class="sxs-lookup"><span data-stu-id="27391-116">children</span></span>|<span data-ttu-id="27391-117">coleção [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="27391-117">[deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md) collection</span></span>|<span data-ttu-id="27391-118">Configurações filhas.</span><span class="sxs-lookup"><span data-stu-id="27391-118">Child settings.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27391-119">Relações</span><span class="sxs-lookup"><span data-stu-id="27391-119">Relationships</span></span>
<span data-ttu-id="27391-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="27391-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27391-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27391-121">JSON Representation</span></span>
<span data-ttu-id="27391-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="27391-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
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
```





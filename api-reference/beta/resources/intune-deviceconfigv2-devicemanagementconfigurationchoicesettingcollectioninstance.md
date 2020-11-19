---
title: tipo de recurso deviceManagementConfigurationChoiceSettingCollectionInstance
description: Configuração de instância dentro da política
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c184daa530de199afc5240b42cbcb1d8204f96df
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241183"
---
# <a name="devicemanagementconfigurationchoicesettingcollectioninstance-resource-type"></a><span data-ttu-id="1af99-103">tipo de recurso deviceManagementConfigurationChoiceSettingCollectionInstance</span><span class="sxs-lookup"><span data-stu-id="1af99-103">deviceManagementConfigurationChoiceSettingCollectionInstance resource type</span></span>

<span data-ttu-id="1af99-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1af99-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1af99-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1af99-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1af99-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1af99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1af99-107">Configuração de instância dentro da política</span><span class="sxs-lookup"><span data-stu-id="1af99-107">Setting instance within policy</span></span>


<span data-ttu-id="1af99-108">Herda de [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="1af99-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1af99-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1af99-109">Properties</span></span>
|<span data-ttu-id="1af99-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1af99-110">Property</span></span>|<span data-ttu-id="1af99-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1af99-111">Type</span></span>|<span data-ttu-id="1af99-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1af99-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1af99-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="1af99-113">settingDefinitionId</span></span>|<span data-ttu-id="1af99-114">String</span><span class="sxs-lookup"><span data-stu-id="1af99-114">String</span></span>|<span data-ttu-id="1af99-115">Definição de ID de definição herdada de [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="1af99-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="1af99-116">choiceSettingCollectionValue</span><span class="sxs-lookup"><span data-stu-id="1af99-116">choiceSettingCollectionValue</span></span>|<span data-ttu-id="1af99-117">coleção [deviceManagementConfigurationChoiceSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="1af99-117">[deviceManagementConfigurationChoiceSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvalue.md) collection</span></span>|<span data-ttu-id="1af99-118">Definição do valor da coleção de opções</span><span class="sxs-lookup"><span data-stu-id="1af99-118">Choice setting collection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="1af99-119">Relações</span><span class="sxs-lookup"><span data-stu-id="1af99-119">Relationships</span></span>
<span data-ttu-id="1af99-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1af99-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1af99-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1af99-121">JSON Representation</span></span>
<span data-ttu-id="1af99-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1af99-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionInstance",
  "settingDefinitionId": "String",
  "choiceSettingCollectionValue": [
    {
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
                                                                  "children": [
                                                                    {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                      "settingDefinitionId": "String",
                                                                      "choiceSettingValue": {
                                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                        "value": null,
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





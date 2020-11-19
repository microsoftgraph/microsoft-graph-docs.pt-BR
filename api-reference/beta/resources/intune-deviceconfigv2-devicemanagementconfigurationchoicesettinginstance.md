---
title: tipo de recurso deviceManagementConfigurationChoiceSettingInstance
description: Configuração de instância dentro da política
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 591c99a1089a9a01acb6b4ded72439f98d3afbb1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241181"
---
# <a name="devicemanagementconfigurationchoicesettinginstance-resource-type"></a><span data-ttu-id="d648e-103">tipo de recurso deviceManagementConfigurationChoiceSettingInstance</span><span class="sxs-lookup"><span data-stu-id="d648e-103">deviceManagementConfigurationChoiceSettingInstance resource type</span></span>

<span data-ttu-id="d648e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d648e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d648e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d648e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d648e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d648e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d648e-107">Configuração de instância dentro da política</span><span class="sxs-lookup"><span data-stu-id="d648e-107">Setting instance within policy</span></span>


<span data-ttu-id="d648e-108">Herda de [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d648e-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d648e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d648e-109">Properties</span></span>
|<span data-ttu-id="d648e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d648e-110">Property</span></span>|<span data-ttu-id="d648e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d648e-111">Type</span></span>|<span data-ttu-id="d648e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d648e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d648e-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="d648e-113">settingDefinitionId</span></span>|<span data-ttu-id="d648e-114">String</span><span class="sxs-lookup"><span data-stu-id="d648e-114">String</span></span>|<span data-ttu-id="d648e-115">Definição de ID de definição herdada de [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d648e-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="d648e-116">choiceSettingValue</span><span class="sxs-lookup"><span data-stu-id="d648e-116">choiceSettingValue</span></span>|[<span data-ttu-id="d648e-117">deviceManagementConfigurationChoiceSettingValue</span><span class="sxs-lookup"><span data-stu-id="d648e-117">deviceManagementConfigurationChoiceSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvalue.md)|<span data-ttu-id="d648e-118">Valor de configuração de opção</span><span class="sxs-lookup"><span data-stu-id="d648e-118">Choice setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="d648e-119">Relações</span><span class="sxs-lookup"><span data-stu-id="d648e-119">Relationships</span></span>
<span data-ttu-id="d648e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d648e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d648e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d648e-121">JSON Representation</span></span>
<span data-ttu-id="d648e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d648e-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
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
                                                                "children": [
                                                                  {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                    "settingDefinitionId": "String",
                                                                    "choiceSettingValue": null
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





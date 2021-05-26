---
title: Tipo de recurso deviceManagementConfigurationOptionDefinition
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cffbb4ccf98637b4fe65b5b593e947fb1dab5c06
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666517"
---
# <a name="devicemanagementconfigurationoptiondefinition-resource-type"></a><span data-ttu-id="25658-103">Tipo de recurso deviceManagementConfigurationOptionDefinition</span><span class="sxs-lookup"><span data-stu-id="25658-103">deviceManagementConfigurationOptionDefinition resource type</span></span>

<span data-ttu-id="25658-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25658-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25658-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="25658-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25658-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25658-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25658-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="25658-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="25658-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25658-108">Properties</span></span>
|<span data-ttu-id="25658-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25658-109">Property</span></span>|<span data-ttu-id="25658-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="25658-110">Type</span></span>|<span data-ttu-id="25658-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="25658-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25658-112">optionValue</span><span class="sxs-lookup"><span data-stu-id="25658-112">optionValue</span></span>|[<span data-ttu-id="25658-113">deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="25658-113">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="25658-114">Valor da opção</span><span class="sxs-lookup"><span data-stu-id="25658-114">Value of the option</span></span>|
|<span data-ttu-id="25658-115">dependentOn</span><span class="sxs-lookup"><span data-stu-id="25658-115">dependentOn</span></span>|<span data-ttu-id="25658-116">[Coleção deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="25658-116">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="25658-117">Lista de configurações dependentes para essa opção</span><span class="sxs-lookup"><span data-stu-id="25658-117">List of dependent settings for this option</span></span>|
|<span data-ttu-id="25658-118">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="25658-118">dependedOnBy</span></span>|<span data-ttu-id="25658-119">[Coleção deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="25658-119">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="25658-120">Lista de Configurações que depende dessa opção</span><span class="sxs-lookup"><span data-stu-id="25658-120">List of Settings that depends on this option</span></span>|
|<span data-ttu-id="25658-121">itemId</span><span class="sxs-lookup"><span data-stu-id="25658-121">itemId</span></span>|<span data-ttu-id="25658-122">String</span><span class="sxs-lookup"><span data-stu-id="25658-122">String</span></span>|<span data-ttu-id="25658-123">Identificador de opção</span><span class="sxs-lookup"><span data-stu-id="25658-123">Identifier of option</span></span>|
|<span data-ttu-id="25658-124">descrição</span><span class="sxs-lookup"><span data-stu-id="25658-124">description</span></span>|<span data-ttu-id="25658-125">String</span><span class="sxs-lookup"><span data-stu-id="25658-125">String</span></span>|<span data-ttu-id="25658-126">Descrição da opção</span><span class="sxs-lookup"><span data-stu-id="25658-126">Description of the option</span></span>|
|<span data-ttu-id="25658-127">helpText</span><span class="sxs-lookup"><span data-stu-id="25658-127">helpText</span></span>|<span data-ttu-id="25658-128">String</span><span class="sxs-lookup"><span data-stu-id="25658-128">String</span></span>|<span data-ttu-id="25658-129">Texto de ajuda da opção</span><span class="sxs-lookup"><span data-stu-id="25658-129">Help text of the option</span></span>|
|<span data-ttu-id="25658-130">nome</span><span class="sxs-lookup"><span data-stu-id="25658-130">name</span></span>|<span data-ttu-id="25658-131">String</span><span class="sxs-lookup"><span data-stu-id="25658-131">String</span></span>|<span data-ttu-id="25658-132">Nome da opção</span><span class="sxs-lookup"><span data-stu-id="25658-132">Name of the option</span></span>|
|<span data-ttu-id="25658-133">displayName</span><span class="sxs-lookup"><span data-stu-id="25658-133">displayName</span></span>|<span data-ttu-id="25658-134">String</span><span class="sxs-lookup"><span data-stu-id="25658-134">String</span></span>|<span data-ttu-id="25658-135">Nome amigável da opção</span><span class="sxs-lookup"><span data-stu-id="25658-135">Friendly name of the option</span></span>|

## <a name="relationships"></a><span data-ttu-id="25658-136">Relações</span><span class="sxs-lookup"><span data-stu-id="25658-136">Relationships</span></span>
<span data-ttu-id="25658-137">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="25658-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="25658-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25658-138">JSON Representation</span></span>
<span data-ttu-id="25658-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25658-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationOptionDefinition",
  "optionValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValue",
    "settingValueTemplateReference": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
      "settingValueTemplateId": "String",
      "useTemplateDefault": true
    },
    "children": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
        "settingDefinitionId": "String",
        "settingInstanceTemplateReference": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
          "settingInstanceTemplateId": "String"
        },
        "choiceSettingValue": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
          "settingValueTemplateReference": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
            "settingValueTemplateId": "String",
            "useTemplateDefault": true
          },
          "value": "String",
          "children": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
              "settingDefinitionId": "String",
              "settingInstanceTemplateReference": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                "settingInstanceTemplateId": "String"
              },
              "choiceSettingValue": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                "settingValueTemplateReference": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                  "settingValueTemplateId": "String",
                  "useTemplateDefault": true
                },
                "value": "String",
                "children": [
                  {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                    "settingDefinitionId": "String",
                    "settingInstanceTemplateReference": {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                      "settingInstanceTemplateId": "String"
                    },
                    "choiceSettingValue": {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                      "settingValueTemplateReference": {
                        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                        "settingValueTemplateId": "String",
                        "useTemplateDefault": true
                      },
                      "value": "String",
                      "children": [
                        {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                          "settingDefinitionId": "String",
                          "settingInstanceTemplateReference": {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                            "settingInstanceTemplateId": "String"
                          },
                          "choiceSettingValue": {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                            "settingValueTemplateReference": {
                              "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                              "settingValueTemplateId": "String",
                              "useTemplateDefault": true
                            },
                            "value": "String",
                            "children": [
                              {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                "settingDefinitionId": "String",
                                "settingInstanceTemplateReference": {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                  "settingInstanceTemplateId": "String"
                                },
                                "choiceSettingValue": {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                  "settingValueTemplateReference": {
                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                    "settingValueTemplateId": "String",
                                    "useTemplateDefault": true
                                  },
                                  "value": "String",
                                  "children": [
                                    {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                      "settingDefinitionId": "String",
                                      "settingInstanceTemplateReference": {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                        "settingInstanceTemplateId": "String"
                                      },
                                      "choiceSettingValue": {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                        "settingValueTemplateReference": {
                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                          "settingValueTemplateId": "String",
                                          "useTemplateDefault": true
                                        },
                                        "value": "String",
                                        "children": [
                                          {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                            "settingDefinitionId": "String",
                                            "settingInstanceTemplateReference": {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                              "settingInstanceTemplateId": "String"
                                            },
                                            "choiceSettingValue": {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                              "settingValueTemplateReference": {
                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                "settingValueTemplateId": "String",
                                                "useTemplateDefault": true
                                              },
                                              "value": "String",
                                              "children": [
                                                {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                  "settingDefinitionId": "String",
                                                  "settingInstanceTemplateReference": {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                    "settingInstanceTemplateId": "String"
                                                  },
                                                  "choiceSettingValue": {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                    "settingValueTemplateReference": {
                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                      "settingValueTemplateId": "String",
                                                      "useTemplateDefault": true
                                                    },
                                                    "value": "String",
                                                    "children": [
                                                      {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                        "settingDefinitionId": "String",
                                                        "settingInstanceTemplateReference": {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                          "settingInstanceTemplateId": "String"
                                                        },
                                                        "choiceSettingValue": {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                          "settingValueTemplateReference": {
                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                            "settingValueTemplateId": "String",
                                                            "useTemplateDefault": true
                                                          },
                                                          "value": "String",
                                                          "children": [
                                                            {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                              "settingDefinitionId": "String",
                                                              "settingInstanceTemplateReference": {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                                "settingInstanceTemplateId": "String"
                                                              },
                                                              "choiceSettingValue": {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                "settingValueTemplateReference": {
                                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                                  "settingValueTemplateId": "String",
                                                                  "useTemplateDefault": true
                                                                },
                                                                "value": "String",
                                                                "children": [
                                                                  {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                    "settingDefinitionId": "String",
                                                                    "settingInstanceTemplateReference": {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                                      "settingInstanceTemplateId": "String"
                                                                    },
                                                                    "choiceSettingValue": {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                      "settingValueTemplateReference": null,
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
  },
  "dependentOn": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn",
      "dependentOn": "String",
      "parentSettingId": "String"
    }
  ],
  "dependedOnBy": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
      "dependedOnBy": "String",
      "required": true
    }
  ],
  "itemId": "String",
  "description": "String",
  "helpText": "String",
  "name": "String",
  "displayName": "String"
}
```





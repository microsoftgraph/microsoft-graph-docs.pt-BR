---
title: tipo de recurso deviceManagementConfigurationOptionDefinition
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5c8ccb388a8feb43b6be96402d45a5b7a0ae62ed
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241163"
---
# <a name="devicemanagementconfigurationoptiondefinition-resource-type"></a><span data-ttu-id="9337a-103">tipo de recurso deviceManagementConfigurationOptionDefinition</span><span class="sxs-lookup"><span data-stu-id="9337a-103">deviceManagementConfigurationOptionDefinition resource type</span></span>

<span data-ttu-id="9337a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9337a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9337a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9337a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9337a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9337a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9337a-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9337a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9337a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9337a-108">Properties</span></span>
|<span data-ttu-id="9337a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9337a-109">Property</span></span>|<span data-ttu-id="9337a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9337a-110">Type</span></span>|<span data-ttu-id="9337a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9337a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9337a-112">optionValue</span><span class="sxs-lookup"><span data-stu-id="9337a-112">optionValue</span></span>|[<span data-ttu-id="9337a-113">deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="9337a-113">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="9337a-114">Valor da opção</span><span class="sxs-lookup"><span data-stu-id="9337a-114">Value of the option</span></span>|
|<span data-ttu-id="9337a-115">dependente</span><span class="sxs-lookup"><span data-stu-id="9337a-115">dependentOn</span></span>|<span data-ttu-id="9337a-116">coleção [deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="9337a-116">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="9337a-117">Lista de configurações dependentes para esta opção</span><span class="sxs-lookup"><span data-stu-id="9337a-117">List of dependent settings for this option</span></span>|
|<span data-ttu-id="9337a-118">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="9337a-118">dependedOnBy</span></span>|<span data-ttu-id="9337a-119">coleção [deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="9337a-119">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="9337a-120">Lista de configurações que depende dessa opção</span><span class="sxs-lookup"><span data-stu-id="9337a-120">List of Settings that depends on this option</span></span>|
|<span data-ttu-id="9337a-121">itemId</span><span class="sxs-lookup"><span data-stu-id="9337a-121">itemId</span></span>|<span data-ttu-id="9337a-122">String</span><span class="sxs-lookup"><span data-stu-id="9337a-122">String</span></span>|<span data-ttu-id="9337a-123">Identificador de opção</span><span class="sxs-lookup"><span data-stu-id="9337a-123">Identifier of option</span></span>|
|<span data-ttu-id="9337a-124">description</span><span class="sxs-lookup"><span data-stu-id="9337a-124">description</span></span>|<span data-ttu-id="9337a-125">String</span><span class="sxs-lookup"><span data-stu-id="9337a-125">String</span></span>|<span data-ttu-id="9337a-126">Descrição da opção</span><span class="sxs-lookup"><span data-stu-id="9337a-126">Description of the option</span></span>|
|<span data-ttu-id="9337a-127">helpText</span><span class="sxs-lookup"><span data-stu-id="9337a-127">helpText</span></span>|<span data-ttu-id="9337a-128">String</span><span class="sxs-lookup"><span data-stu-id="9337a-128">String</span></span>|<span data-ttu-id="9337a-129">Texto de ajuda da opção</span><span class="sxs-lookup"><span data-stu-id="9337a-129">Help text of the option</span></span>|
|<span data-ttu-id="9337a-130">nome</span><span class="sxs-lookup"><span data-stu-id="9337a-130">name</span></span>|<span data-ttu-id="9337a-131">String</span><span class="sxs-lookup"><span data-stu-id="9337a-131">String</span></span>|<span data-ttu-id="9337a-132">Nome da opção</span><span class="sxs-lookup"><span data-stu-id="9337a-132">Name of the option</span></span>|
|<span data-ttu-id="9337a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9337a-133">displayName</span></span>|<span data-ttu-id="9337a-134">String</span><span class="sxs-lookup"><span data-stu-id="9337a-134">String</span></span>|<span data-ttu-id="9337a-135">Nome amigável da opção</span><span class="sxs-lookup"><span data-stu-id="9337a-135">Friendly name of the option</span></span>|

## <a name="relationships"></a><span data-ttu-id="9337a-136">Relações</span><span class="sxs-lookup"><span data-stu-id="9337a-136">Relationships</span></span>
<span data-ttu-id="9337a-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9337a-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9337a-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9337a-138">JSON Representation</span></span>
<span data-ttu-id="9337a-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9337a-139">Here is a JSON representation of the resource.</span></span>
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





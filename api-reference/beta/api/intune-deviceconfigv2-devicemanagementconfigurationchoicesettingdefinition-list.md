---
title: Listar deviceManagementConfigurationChoiceSettingDefinitions
description: Listar propriedades e relações dos objetos deviceManagementConfigurationChoiceSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c5a6eb5cabbf7d430892f77d43d1050099c177c6
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864422"
---
# <a name="list-devicemanagementconfigurationchoicesettingdefinitions"></a><span data-ttu-id="b070b-103">Listar deviceManagementConfigurationChoiceSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="b070b-103">List deviceManagementConfigurationChoiceSettingDefinitions</span></span>

<span data-ttu-id="b070b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b070b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b070b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b070b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b070b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b070b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b070b-107">Listar propriedades e relações dos [objetos deviceManagementConfigurationChoiceSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b070b-107">List properties and relationships of the [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b070b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b070b-108">Prerequisites</span></span>
<span data-ttu-id="b070b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b070b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b070b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b070b-111">Permission type</span></span>|<span data-ttu-id="b070b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b070b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b070b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b070b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b070b-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b070b-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b070b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b070b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b070b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b070b-116">Not supported.</span></span>|
|<span data-ttu-id="b070b-117">Application</span><span class="sxs-lookup"><span data-stu-id="b070b-117">Application</span></span>|<span data-ttu-id="b070b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b070b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b070b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b070b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reusableSettings
GET /deviceManagement/configurationSettings
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="b070b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b070b-120">Request headers</span></span>
|<span data-ttu-id="b070b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b070b-121">Header</span></span>|<span data-ttu-id="b070b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b070b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b070b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b070b-123">Authorization</span></span>|<span data-ttu-id="b070b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b070b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b070b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b070b-125">Accept</span></span>|<span data-ttu-id="b070b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b070b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b070b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b070b-127">Request body</span></span>
<span data-ttu-id="b070b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b070b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b070b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b070b-129">Response</span></span>
<span data-ttu-id="b070b-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b070b-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b070b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b070b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b070b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b070b-132">Request</span></span>
<span data-ttu-id="b070b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b070b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reusableSettings
```

### <a name="response"></a><span data-ttu-id="b070b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b070b-134">Response</span></span>
<span data-ttu-id="b070b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b070b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10952

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingDefinition",
      "applicability": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
        "description": "Description value",
        "platform": "macOS",
        "deviceMode": "kiosk",
        "technologies": "mdm"
      },
      "accessTypes": "add",
      "keywords": [
        "Keywords value"
      ],
      "infoUrls": [
        "Info Urls value"
      ],
      "occurrence": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
        "minDeviceOccurrence": 3,
        "maxDeviceOccurrence": 3
      },
      "baseUri": "Base Uri value",
      "offsetUri": "Offset Uri value",
      "rootDefinitionId": "Root Definition Id value",
      "categoryId": "Category Id value",
      "settingUsage": "configuration",
      "uxBehavior": "dropdown",
      "visibility": "settingsCatalog",
      "referredSettingInformationList": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
          "settingDefinitionId": "Setting Definition Id value"
        }
      ],
      "id": "30b2258a-258a-30b2-8a25-b2308a25b230",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value",
      "version": "Version value",
      "options": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinition",
          "optionValue": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValue",
            "children": [
              {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                "settingDefinitionId": "Setting Definition Id value",
                "choiceSettingValue": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                  "value": "Value value",
                  "children": [
                    {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                      "settingDefinitionId": "Setting Definition Id value",
                      "choiceSettingValue": {
                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                        "value": "Value value",
                        "children": [
                          {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                            "settingDefinitionId": "Setting Definition Id value",
                            "choiceSettingValue": {
                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                              "value": "Value value",
                              "children": [
                                {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                  "settingDefinitionId": "Setting Definition Id value",
                                  "choiceSettingValue": {
                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                    "value": "Value value",
                                    "children": [
                                      {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                        "settingDefinitionId": "Setting Definition Id value",
                                        "choiceSettingValue": {
                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                          "value": "Value value",
                                          "children": [
                                            {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                              "settingDefinitionId": "Setting Definition Id value",
                                              "choiceSettingValue": {
                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                "value": "Value value",
                                                "children": [
                                                  {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                    "settingDefinitionId": "Setting Definition Id value",
                                                    "choiceSettingValue": {
                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                      "value": "Value value",
                                                      "children": [
                                                        {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                          "settingDefinitionId": "Setting Definition Id value",
                                                          "choiceSettingValue": {
                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                            "value": "Value value",
                                                            "children": [
                                                              {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                "settingDefinitionId": "Setting Definition Id value",
                                                                "choiceSettingValue": {
                                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                  "value": "Value value",
                                                                  "children": [
                                                                    {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                      "settingDefinitionId": "Setting Definition Id value",
                                                                      "choiceSettingValue": {
                                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                        "value": "Value value",
                                                                        "children": [
                                                                          {
                                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                            "settingDefinitionId": "Setting Definition Id value",
                                                                            "choiceSettingValue": {
                                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                              "value": "Value value",
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
              "dependentOn": "Dependent On value",
              "parentSettingId": "Parent Setting Id value"
            }
          ],
          "dependedOnBy": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
              "dependedOnBy": "Depended On By value",
              "required": true
            }
          ],
          "itemId": "Item Id value",
          "description": "Description value",
          "helpText": "Help Text value",
          "name": "Name value",
          "displayName": "Display Name value"
        }
      ],
      "defaultOptionId": "Default Option Id value"
    }
  ]
}
```





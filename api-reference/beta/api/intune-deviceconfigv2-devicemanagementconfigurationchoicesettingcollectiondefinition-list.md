---
title: Listar deviceManagementConfigurationChoiceSettingCollectionDefinitions
description: Listar propriedades e relações dos objetos deviceManagementConfigurationChoiceSettingCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f5bf59398c7379f36ccfc2ce3713ea4f2da3a8e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666145"
---
# <a name="list-devicemanagementconfigurationchoicesettingcollectiondefinitions"></a><span data-ttu-id="4825c-103">Listar deviceManagementConfigurationChoiceSettingCollectionDefinitions</span><span class="sxs-lookup"><span data-stu-id="4825c-103">List deviceManagementConfigurationChoiceSettingCollectionDefinitions</span></span>

<span data-ttu-id="4825c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4825c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4825c-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4825c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4825c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4825c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4825c-107">Listar propriedades e relações [dos objetos deviceManagementConfigurationChoiceSettingCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4825c-107">List properties and relationships of the [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4825c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4825c-108">Prerequisites</span></span>
<span data-ttu-id="4825c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4825c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4825c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4825c-111">Permission type</span></span>|<span data-ttu-id="4825c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4825c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4825c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4825c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4825c-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4825c-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4825c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4825c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4825c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4825c-116">Not supported.</span></span>|
|<span data-ttu-id="4825c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4825c-117">Application</span></span>|<span data-ttu-id="4825c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4825c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4825c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4825c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reusableSettings
GET /deviceManagement/configurationSettings
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
GET /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates/{deviceManagementConfigurationSettingTemplateId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="4825c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4825c-120">Request headers</span></span>
|<span data-ttu-id="4825c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4825c-121">Header</span></span>|<span data-ttu-id="4825c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4825c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4825c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4825c-123">Authorization</span></span>|<span data-ttu-id="4825c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4825c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4825c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4825c-125">Accept</span></span>|<span data-ttu-id="4825c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4825c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4825c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4825c-127">Request body</span></span>
<span data-ttu-id="4825c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4825c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4825c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4825c-129">Response</span></span>
<span data-ttu-id="4825c-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4825c-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4825c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4825c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4825c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4825c-132">Request</span></span>
<span data-ttu-id="4825c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4825c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reusableSettings
```

### <a name="response"></a><span data-ttu-id="4825c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4825c-134">Response</span></span>
<span data-ttu-id="4825c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4825c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 20319

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionDefinition",
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
      "id": "eb03fdca-fdca-eb03-cafd-03ebcafd03eb",
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
            "settingValueTemplateReference": {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
              "settingValueTemplateId": "Setting Value Template Id value",
              "useTemplateDefault": true
            },
            "children": [
              {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                "settingDefinitionId": "Setting Definition Id value",
                "settingInstanceTemplateReference": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                  "settingInstanceTemplateId": "Setting Instance Template Id value"
                },
                "choiceSettingValue": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                  "settingValueTemplateReference": {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                    "settingValueTemplateId": "Setting Value Template Id value",
                    "useTemplateDefault": true
                  },
                  "value": "Value value",
                  "children": [
                    {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                      "settingDefinitionId": "Setting Definition Id value",
                      "settingInstanceTemplateReference": {
                        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                        "settingInstanceTemplateId": "Setting Instance Template Id value"
                      },
                      "choiceSettingValue": {
                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                        "settingValueTemplateReference": {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                          "settingValueTemplateId": "Setting Value Template Id value",
                          "useTemplateDefault": true
                        },
                        "value": "Value value",
                        "children": [
                          {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                            "settingDefinitionId": "Setting Definition Id value",
                            "settingInstanceTemplateReference": {
                              "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                              "settingInstanceTemplateId": "Setting Instance Template Id value"
                            },
                            "choiceSettingValue": {
                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                              "settingValueTemplateReference": {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                "settingValueTemplateId": "Setting Value Template Id value",
                                "useTemplateDefault": true
                              },
                              "value": "Value value",
                              "children": [
                                {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                  "settingDefinitionId": "Setting Definition Id value",
                                  "settingInstanceTemplateReference": {
                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                    "settingInstanceTemplateId": "Setting Instance Template Id value"
                                  },
                                  "choiceSettingValue": {
                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                    "settingValueTemplateReference": {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                      "settingValueTemplateId": "Setting Value Template Id value",
                                      "useTemplateDefault": true
                                    },
                                    "value": "Value value",
                                    "children": [
                                      {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                        "settingDefinitionId": "Setting Definition Id value",
                                        "settingInstanceTemplateReference": {
                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                          "settingInstanceTemplateId": "Setting Instance Template Id value"
                                        },
                                        "choiceSettingValue": {
                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                          "settingValueTemplateReference": {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                            "settingValueTemplateId": "Setting Value Template Id value",
                                            "useTemplateDefault": true
                                          },
                                          "value": "Value value",
                                          "children": [
                                            {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                              "settingDefinitionId": "Setting Definition Id value",
                                              "settingInstanceTemplateReference": {
                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                "settingInstanceTemplateId": "Setting Instance Template Id value"
                                              },
                                              "choiceSettingValue": {
                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                "settingValueTemplateReference": {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                  "settingValueTemplateId": "Setting Value Template Id value",
                                                  "useTemplateDefault": true
                                                },
                                                "value": "Value value",
                                                "children": [
                                                  {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                    "settingDefinitionId": "Setting Definition Id value",
                                                    "settingInstanceTemplateReference": {
                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                      "settingInstanceTemplateId": "Setting Instance Template Id value"
                                                    },
                                                    "choiceSettingValue": {
                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                      "settingValueTemplateReference": {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                        "settingValueTemplateId": "Setting Value Template Id value",
                                                        "useTemplateDefault": true
                                                      },
                                                      "value": "Value value",
                                                      "children": [
                                                        {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                          "settingDefinitionId": "Setting Definition Id value",
                                                          "settingInstanceTemplateReference": {
                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                            "settingInstanceTemplateId": "Setting Instance Template Id value"
                                                          },
                                                          "choiceSettingValue": {
                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                            "settingValueTemplateReference": {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                              "settingValueTemplateId": "Setting Value Template Id value",
                                                              "useTemplateDefault": true
                                                            },
                                                            "value": "Value value",
                                                            "children": [
                                                              {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                "settingDefinitionId": "Setting Definition Id value",
                                                                "settingInstanceTemplateReference": {
                                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                                  "settingInstanceTemplateId": "Setting Instance Template Id value"
                                                                },
                                                                "choiceSettingValue": {
                                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                  "settingValueTemplateReference": {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                                    "settingValueTemplateId": "Setting Value Template Id value",
                                                                    "useTemplateDefault": true
                                                                  },
                                                                  "value": "Value value",
                                                                  "children": [
                                                                    {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                      "settingDefinitionId": "Setting Definition Id value",
                                                                      "settingInstanceTemplateReference": {
                                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                                        "settingInstanceTemplateId": "Setting Instance Template Id value"
                                                                      },
                                                                      "choiceSettingValue": {
                                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                        "settingValueTemplateReference": {
                                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                                          "settingValueTemplateId": "Setting Value Template Id value",
                                                                          "useTemplateDefault": true
                                                                        },
                                                                        "value": "Value value",
                                                                        "children": [
                                                                          {
                                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                            "settingDefinitionId": "Setting Definition Id value",
                                                                            "settingInstanceTemplateReference": {
                                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                                              "settingInstanceTemplateId": "Setting Instance Template Id value"
                                                                            },
                                                                            "choiceSettingValue": {
                                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                              "settingValueTemplateReference": null,
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
      "defaultOptionId": "Default Option Id value",
      "maximumCount": 12,
      "minimumCount": 12
    }
  ]
}
```





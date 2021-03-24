---
title: Obter deviceManagementConfigurationSimpleSettingCollectionDefinition
description: Leia propriedades e relações do objeto deviceManagementConfigurationSimpleSettingCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a15f4f1ed0e5b268dcd391ee430a2e0e4fd1e1a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129164"
---
# <a name="get-devicemanagementconfigurationsimplesettingcollectiondefinition"></a><span data-ttu-id="a1282-103">Obter deviceManagementConfigurationSimpleSettingCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="a1282-103">Get deviceManagementConfigurationSimpleSettingCollectionDefinition</span></span>

<span data-ttu-id="a1282-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1282-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1282-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1282-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1282-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1282-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1282-107">Leia propriedades e relações do [objeto deviceManagementConfigurationSimpleSettingCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a1282-107">Read properties and relationships of the [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1282-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1282-108">Prerequisites</span></span>
<span data-ttu-id="a1282-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1282-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1282-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1282-111">Permission type</span></span>|<span data-ttu-id="a1282-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1282-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1282-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1282-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1282-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1282-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1282-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1282-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1282-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1282-116">Not supported.</span></span>|
|<span data-ttu-id="a1282-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1282-117">Application</span></span>|<span data-ttu-id="a1282-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1282-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1282-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1282-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1282-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a1282-120">Optional query parameters</span></span>
<span data-ttu-id="a1282-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a1282-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1282-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1282-122">Request headers</span></span>
|<span data-ttu-id="a1282-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1282-123">Header</span></span>|<span data-ttu-id="a1282-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a1282-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1282-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1282-125">Authorization</span></span>|<span data-ttu-id="a1282-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1282-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1282-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1282-127">Accept</span></span>|<span data-ttu-id="a1282-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a1282-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1282-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1282-129">Request body</span></span>
<span data-ttu-id="a1282-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1282-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1282-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1282-131">Response</span></span>
<span data-ttu-id="a1282-132">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1282-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1282-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1282-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1282-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1282-134">Request</span></span>
<span data-ttu-id="a1282-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1282-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="a1282-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1282-136">Response</span></span>
<span data-ttu-id="a1282-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1282-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9648

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionDefinition",
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
    "id": "cb4abda1-bda1-cb4a-a1bd-4acba1bd4acb",
    "description": "Description value",
    "helpText": "Help Text value",
    "name": "Name value",
    "displayName": "Display Name value",
    "version": "Version value",
    "valueDefinition": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueDefinition"
    },
    "defaultValue": {
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
    "maximumCount": 12,
    "minimumCount": 12
  }
}
```





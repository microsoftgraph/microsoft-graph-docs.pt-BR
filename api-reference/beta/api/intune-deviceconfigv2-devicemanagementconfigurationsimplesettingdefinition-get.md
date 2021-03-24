---
title: Obter deviceManagementConfigurationSimpleSettingDefinition
description: Leia propriedades e relações do objeto deviceManagementConfigurationSimpleSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efeaceab7cea80f91b4a68df4ced835444e0779c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129101"
---
# <a name="get-devicemanagementconfigurationsimplesettingdefinition"></a><span data-ttu-id="0eb85-103">Obter deviceManagementConfigurationSimpleSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="0eb85-103">Get deviceManagementConfigurationSimpleSettingDefinition</span></span>

<span data-ttu-id="0eb85-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0eb85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0eb85-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0eb85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0eb85-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0eb85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0eb85-107">Leia propriedades e relações do [objeto deviceManagementConfigurationSimpleSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0eb85-107">Read properties and relationships of the [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0eb85-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0eb85-108">Prerequisites</span></span>
<span data-ttu-id="0eb85-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0eb85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0eb85-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0eb85-111">Permission type</span></span>|<span data-ttu-id="0eb85-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0eb85-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0eb85-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0eb85-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0eb85-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eb85-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0eb85-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0eb85-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0eb85-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0eb85-116">Not supported.</span></span>|
|<span data-ttu-id="0eb85-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0eb85-117">Application</span></span>|<span data-ttu-id="0eb85-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eb85-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0eb85-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0eb85-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0eb85-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0eb85-120">Optional query parameters</span></span>
<span data-ttu-id="0eb85-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0eb85-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0eb85-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0eb85-122">Request headers</span></span>
|<span data-ttu-id="0eb85-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0eb85-123">Header</span></span>|<span data-ttu-id="0eb85-124">Valor</span><span class="sxs-lookup"><span data-stu-id="0eb85-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0eb85-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0eb85-125">Authorization</span></span>|<span data-ttu-id="0eb85-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0eb85-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0eb85-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0eb85-127">Accept</span></span>|<span data-ttu-id="0eb85-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0eb85-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0eb85-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0eb85-129">Request body</span></span>
<span data-ttu-id="0eb85-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0eb85-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0eb85-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0eb85-131">Response</span></span>
<span data-ttu-id="0eb85-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0eb85-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0eb85-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0eb85-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0eb85-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0eb85-134">Request</span></span>
<span data-ttu-id="0eb85-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0eb85-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="0eb85-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0eb85-136">Response</span></span>
<span data-ttu-id="0eb85-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0eb85-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9588

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingDefinition",
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
    "id": "30dc0613-0613-30dc-1306-dc301306dc30",
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
    ]
  }
}
```





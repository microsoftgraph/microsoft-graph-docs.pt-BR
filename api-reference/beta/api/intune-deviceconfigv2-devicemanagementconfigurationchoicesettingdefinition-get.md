---
title: Obter deviceManagementConfigurationChoiceSettingDefinition
description: Leia as propriedades e as relações do objeto deviceManagementConfigurationChoiceSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 91909aca893328557f3542d961fc690960980b1d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241217"
---
# <a name="get-devicemanagementconfigurationchoicesettingdefinition"></a><span data-ttu-id="64572-103">Obter deviceManagementConfigurationChoiceSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="64572-103">Get deviceManagementConfigurationChoiceSettingDefinition</span></span>

<span data-ttu-id="64572-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64572-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64572-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64572-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64572-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64572-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64572-107">Leia as propriedades e as relações do objeto [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="64572-107">Read properties and relationships of the [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64572-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64572-108">Prerequisites</span></span>
<span data-ttu-id="64572-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64572-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64572-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64572-111">Permission type</span></span>|<span data-ttu-id="64572-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64572-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64572-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64572-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64572-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="64572-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="64572-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64572-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64572-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64572-116">Not supported.</span></span>|
|<span data-ttu-id="64572-117">Application</span><span class="sxs-lookup"><span data-stu-id="64572-117">Application</span></span>|<span data-ttu-id="64572-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="64572-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64572-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64572-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64572-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="64572-120">Optional query parameters</span></span>
<span data-ttu-id="64572-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="64572-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64572-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64572-122">Request headers</span></span>
|<span data-ttu-id="64572-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64572-123">Header</span></span>|<span data-ttu-id="64572-124">Valor</span><span class="sxs-lookup"><span data-stu-id="64572-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64572-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="64572-125">Authorization</span></span>|<span data-ttu-id="64572-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64572-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64572-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64572-127">Accept</span></span>|<span data-ttu-id="64572-128">application/json</span><span class="sxs-lookup"><span data-stu-id="64572-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64572-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64572-129">Request body</span></span>
<span data-ttu-id="64572-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64572-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64572-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="64572-131">Response</span></span>
<span data-ttu-id="64572-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64572-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64572-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64572-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="64572-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64572-134">Request</span></span>
<span data-ttu-id="64572-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64572-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="64572-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="64572-136">Response</span></span>
<span data-ttu-id="64572-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64572-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10285

{
  "value": {
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
}
```





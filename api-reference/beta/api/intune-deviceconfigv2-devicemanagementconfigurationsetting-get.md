---
title: Obter deviceManagementConfigurationSetting
description: Leia propriedades e relações do objeto deviceManagementConfigurationSetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 03acd2cebb61a5cb47300dd10409a2c48c60c5d1
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666419"
---
# <a name="get-devicemanagementconfigurationsetting"></a><span data-ttu-id="dafac-103">Obter deviceManagementConfigurationSetting</span><span class="sxs-lookup"><span data-stu-id="dafac-103">Get deviceManagementConfigurationSetting</span></span>

<span data-ttu-id="dafac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dafac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dafac-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dafac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dafac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dafac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dafac-107">Leia propriedades e relações do [objeto deviceManagementConfigurationSetting.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)</span><span class="sxs-lookup"><span data-stu-id="dafac-107">Read properties and relationships of the [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dafac-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dafac-108">Prerequisites</span></span>
<span data-ttu-id="dafac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dafac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dafac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dafac-111">Permission type</span></span>|<span data-ttu-id="dafac-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dafac-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dafac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dafac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dafac-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dafac-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dafac-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dafac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dafac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dafac-116">Not supported.</span></span>|
|<span data-ttu-id="dafac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dafac-117">Application</span></span>|<span data-ttu-id="dafac-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dafac-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dafac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dafac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dafac-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dafac-120">Optional query parameters</span></span>
<span data-ttu-id="dafac-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dafac-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dafac-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dafac-122">Request headers</span></span>
|<span data-ttu-id="dafac-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dafac-123">Header</span></span>|<span data-ttu-id="dafac-124">Valor</span><span class="sxs-lookup"><span data-stu-id="dafac-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dafac-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="dafac-125">Authorization</span></span>|<span data-ttu-id="dafac-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dafac-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dafac-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dafac-127">Accept</span></span>|<span data-ttu-id="dafac-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dafac-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dafac-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dafac-129">Request body</span></span>
<span data-ttu-id="dafac-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dafac-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dafac-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dafac-131">Response</span></span>
<span data-ttu-id="dafac-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dafac-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dafac-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dafac-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="dafac-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dafac-134">Request</span></span>
<span data-ttu-id="dafac-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dafac-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}
```

### <a name="response"></a><span data-ttu-id="dafac-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dafac-136">Response</span></span>
<span data-ttu-id="dafac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dafac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 16631

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementConfigurationSetting",
    "id": "9acf977e-977e-9acf-7e97-cf9a7e97cf9a",
    "settingInstance": {
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
                                                                    "settingValueTemplateReference": {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                                      "settingValueTemplateId": "Setting Value Template Id value",
                                                                      "useTemplateDefault": true
                                                                    },
                                                                    "value": "Value value",
                                                                    "children": [
                                                                      {
                                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                        "settingDefinitionId": null,
                                                                        "settingInstanceTemplateReference": null,
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
  }
}
```





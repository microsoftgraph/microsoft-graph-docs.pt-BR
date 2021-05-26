---
title: Obter deviceManagementReusablePolicySetting
description: Leia propriedades e relações do objeto deviceManagementReusablePolicySetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 03ee8463f60100850a8334f7af7079dfc960ab8e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665410"
---
# <a name="get-devicemanagementreusablepolicysetting"></a><span data-ttu-id="7276d-103">Obter deviceManagementReusablePolicySetting</span><span class="sxs-lookup"><span data-stu-id="7276d-103">Get deviceManagementReusablePolicySetting</span></span>

<span data-ttu-id="7276d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7276d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7276d-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7276d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7276d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7276d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7276d-107">Leia propriedades e relações do [objeto deviceManagementReusablePolicySetting.](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)</span><span class="sxs-lookup"><span data-stu-id="7276d-107">Read properties and relationships of the [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7276d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7276d-108">Prerequisites</span></span>
<span data-ttu-id="7276d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7276d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7276d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7276d-111">Permission type</span></span>|<span data-ttu-id="7276d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7276d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7276d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7276d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7276d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7276d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7276d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7276d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7276d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7276d-116">Not supported.</span></span>|
|<span data-ttu-id="7276d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7276d-117">Application</span></span>|<span data-ttu-id="7276d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7276d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7276d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7276d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7276d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7276d-120">Optional query parameters</span></span>
<span data-ttu-id="7276d-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7276d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7276d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7276d-122">Request headers</span></span>
|<span data-ttu-id="7276d-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7276d-123">Header</span></span>|<span data-ttu-id="7276d-124">Valor</span><span class="sxs-lookup"><span data-stu-id="7276d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7276d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7276d-125">Authorization</span></span>|<span data-ttu-id="7276d-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7276d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7276d-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7276d-127">Accept</span></span>|<span data-ttu-id="7276d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7276d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7276d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7276d-129">Request body</span></span>
<span data-ttu-id="7276d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7276d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7276d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7276d-131">Response</span></span>
<span data-ttu-id="7276d-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7276d-132">If successful, this method returns a `200 OK` response code and [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7276d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7276d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7276d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7276d-134">Request</span></span>
<span data-ttu-id="7276d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7276d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}
```

### <a name="response"></a><span data-ttu-id="7276d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7276d-136">Response</span></span>
<span data-ttu-id="7276d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7276d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 16967

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementReusablePolicySetting",
    "id": "7a4f9bd7-9bd7-7a4f-d79b-4f7ad79b4f7a",
    "displayName": "Display Name value",
    "description": "Description value",
    "settingDefinitionId": "Setting Definition Id value",
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
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7,
    "referencingConfigurationPolicyCount": 3
  }
}
```





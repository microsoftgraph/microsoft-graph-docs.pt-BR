---
title: ação clone
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 106f2597cf2530de1378201a756633426cb6bb1a
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58807108"
---
# <a name="clone-action"></a>ação clone

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}/clone
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, essa ação retornará um código de resposta e `200 OK` um [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}/clone
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 16942

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
                                                                  "settingDefinitionId": null,
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




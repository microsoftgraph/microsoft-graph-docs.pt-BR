---
title: Atualizar deviceManagementConfigurationSetting
description: Atualize as propriedades de um objeto deviceManagementConfigurationSetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d6f710798ab3cf077c2db4e853ae76b2b2c593d1
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670271"
---
# <a name="update-devicemanagementconfigurationsetting"></a>Atualizar deviceManagementConfigurationSetting

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/compliancePolicies/{deviceManagementCompliancePolicyId}/settings/{deviceManagementConfigurationSettingId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave dessa configuração dentro da política que a contém. Gerado automaticamente.|
|settingInstance|[deviceManagementConfigurationSettingInstance](../resources/intune-shared-devicemanagementconfigurationsettinginstance.md)|Instância de Configuração|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/compliancePolicies/{deviceManagementCompliancePolicyId}/settings/{deviceManagementConfigurationSettingId}
Content-type: application/json
Content-length: 16129

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSetting",
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
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 16178

{
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
```





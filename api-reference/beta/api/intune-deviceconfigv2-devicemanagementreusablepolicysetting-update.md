---
title: Atualizar deviceManagementReusablePolicySetting
description: Atualize as propriedades de um objeto deviceManagementReusablePolicySetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 06a15428fe3bd67d9b8566568de855329aacf074
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665536"
---
# <a name="update-devicemanagementreusablepolicysetting"></a><span data-ttu-id="75539-103">Atualizar deviceManagementReusablePolicySetting</span><span class="sxs-lookup"><span data-stu-id="75539-103">Update deviceManagementReusablePolicySetting</span></span>

<span data-ttu-id="75539-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75539-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75539-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75539-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75539-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75539-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75539-107">Atualize as propriedades de [um objeto deviceManagementReusablePolicySetting.](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)</span><span class="sxs-lookup"><span data-stu-id="75539-107">Update the properties of a [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75539-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="75539-108">Prerequisites</span></span>
<span data-ttu-id="75539-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75539-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75539-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75539-111">Permission type</span></span>|<span data-ttu-id="75539-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75539-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75539-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75539-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75539-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75539-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75539-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75539-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75539-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75539-116">Not supported.</span></span>|
|<span data-ttu-id="75539-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75539-117">Application</span></span>|<span data-ttu-id="75539-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75539-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75539-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75539-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}
```

## <a name="request-headers"></a><span data-ttu-id="75539-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75539-120">Request headers</span></span>
|<span data-ttu-id="75539-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75539-121">Header</span></span>|<span data-ttu-id="75539-122">Valor</span><span class="sxs-lookup"><span data-stu-id="75539-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75539-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="75539-123">Authorization</span></span>|<span data-ttu-id="75539-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75539-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75539-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="75539-125">Accept</span></span>|<span data-ttu-id="75539-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75539-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75539-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75539-127">Request body</span></span>
<span data-ttu-id="75539-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementReusablePolicySetting.](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)</span><span class="sxs-lookup"><span data-stu-id="75539-128">In the request body, supply a JSON representation for the [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object.</span></span>

<span data-ttu-id="75539-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md).</span><span class="sxs-lookup"><span data-stu-id="75539-129">The following table shows the properties that are required when you create the [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md).</span></span>

|<span data-ttu-id="75539-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75539-130">Property</span></span>|<span data-ttu-id="75539-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="75539-131">Type</span></span>|<span data-ttu-id="75539-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="75539-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75539-133">id</span><span class="sxs-lookup"><span data-stu-id="75539-133">id</span></span>|<span data-ttu-id="75539-134">String</span><span class="sxs-lookup"><span data-stu-id="75539-134">String</span></span>|<span data-ttu-id="75539-135">id de configuração reutilizável gerada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="75539-135">system generated reusable setting id.</span></span>|
|<span data-ttu-id="75539-136">displayName</span><span class="sxs-lookup"><span data-stu-id="75539-136">displayName</span></span>|<span data-ttu-id="75539-137">String</span><span class="sxs-lookup"><span data-stu-id="75539-137">String</span></span>|<span data-ttu-id="75539-138">nome de exibição de configuração reutilizável fornecido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="75539-138">reusable setting display name supplied by user.</span></span>|
|<span data-ttu-id="75539-139">descrição</span><span class="sxs-lookup"><span data-stu-id="75539-139">description</span></span>|<span data-ttu-id="75539-140">String</span><span class="sxs-lookup"><span data-stu-id="75539-140">String</span></span>|<span data-ttu-id="75539-141">descrição da configuração reutilizável fornecida pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="75539-141">reusable setting description supplied by user.</span></span>|
|<span data-ttu-id="75539-142">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="75539-142">settingDefinitionId</span></span>|<span data-ttu-id="75539-143">String</span><span class="sxs-lookup"><span data-stu-id="75539-143">String</span></span>|<span data-ttu-id="75539-144">id de definição de definição associada a essa configuração reutilizável.</span><span class="sxs-lookup"><span data-stu-id="75539-144">setting definition id associated with this reusable setting.</span></span>|
|<span data-ttu-id="75539-145">settingInstance</span><span class="sxs-lookup"><span data-stu-id="75539-145">settingInstance</span></span>|[<span data-ttu-id="75539-146">deviceManagementConfigurationSettingInstance</span><span class="sxs-lookup"><span data-stu-id="75539-146">deviceManagementConfigurationSettingInstance</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|<span data-ttu-id="75539-147">instância de configuração de configuração reutilizável</span><span class="sxs-lookup"><span data-stu-id="75539-147">reusable setting configuration instance</span></span>|
|<span data-ttu-id="75539-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75539-148">createdDateTime</span></span>|<span data-ttu-id="75539-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75539-149">DateTimeOffset</span></span>|<span data-ttu-id="75539-150">reutilizável definindo data e hora de criação.</span><span class="sxs-lookup"><span data-stu-id="75539-150">reusable setting creation date and time.</span></span> <span data-ttu-id="75539-151">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="75539-151">This property is read-only.</span></span>|
|<span data-ttu-id="75539-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75539-152">lastModifiedDateTime</span></span>|<span data-ttu-id="75539-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75539-153">DateTimeOffset</span></span>|<span data-ttu-id="75539-154">data e hora em que a configuração reutilizável foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="75539-154">date and time when reusable setting was last modified.</span></span> <span data-ttu-id="75539-155">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="75539-155">This property is read-only.</span></span>|
|<span data-ttu-id="75539-156">versão</span><span class="sxs-lookup"><span data-stu-id="75539-156">version</span></span>|<span data-ttu-id="75539-157">Int32</span><span class="sxs-lookup"><span data-stu-id="75539-157">Int32</span></span>|<span data-ttu-id="75539-158">número de versão para configuração reutilizável.</span><span class="sxs-lookup"><span data-stu-id="75539-158">version number for reusable setting.</span></span> <span data-ttu-id="75539-159">Valores válidos de 0 a 2147483647.</span><span class="sxs-lookup"><span data-stu-id="75539-159">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="75539-160">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="75539-160">This property is read-only.</span></span>|
|<span data-ttu-id="75539-161">referencingConfigurationPolicyCount</span><span class="sxs-lookup"><span data-stu-id="75539-161">referencingConfigurationPolicyCount</span></span>|<span data-ttu-id="75539-162">Int32</span><span class="sxs-lookup"><span data-stu-id="75539-162">Int32</span></span>|<span data-ttu-id="75539-163">contagem de políticas de configuração fazendo referência à configuração atual reutilizável.</span><span class="sxs-lookup"><span data-stu-id="75539-163">count of configuration policies referencing the current reusable setting.</span></span> <span data-ttu-id="75539-164">Valores válidos de 0 a 2147483647.</span><span class="sxs-lookup"><span data-stu-id="75539-164">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="75539-165">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="75539-165">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="75539-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="75539-166">Response</span></span>
<span data-ttu-id="75539-167">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75539-167">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75539-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75539-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="75539-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75539-169">Request</span></span>
<span data-ttu-id="75539-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75539-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}
Content-type: application/json
Content-length: 16328

{
  "@odata.type": "#microsoft.graph.deviceManagementReusablePolicySetting",
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
  "version": 7,
  "referencingConfigurationPolicyCount": 3
}
```

### <a name="response"></a><span data-ttu-id="75539-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="75539-171">Response</span></span>
<span data-ttu-id="75539-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75539-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 16500

{
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
```





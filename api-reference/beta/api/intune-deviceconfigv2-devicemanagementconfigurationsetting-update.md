---
title: Atualizar deviceManagementConfigurationSetting
description: Atualiza as propriedades de um objeto deviceManagementConfigurationSetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: abbf6165a043d18d965c2dd6343908dc3726e572
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241365"
---
# <a name="update-devicemanagementconfigurationsetting"></a><span data-ttu-id="f64ce-103">Atualizar deviceManagementConfigurationSetting</span><span class="sxs-lookup"><span data-stu-id="f64ce-103">Update deviceManagementConfigurationSetting</span></span>

<span data-ttu-id="f64ce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f64ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f64ce-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f64ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f64ce-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f64ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f64ce-107">Atualiza as propriedades de um objeto [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="f64ce-107">Update the properties of a [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f64ce-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f64ce-108">Prerequisites</span></span>
<span data-ttu-id="f64ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f64ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f64ce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f64ce-111">Permission type</span></span>|<span data-ttu-id="f64ce-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f64ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f64ce-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f64ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f64ce-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f64ce-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f64ce-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f64ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f64ce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f64ce-116">Not supported.</span></span>|
|<span data-ttu-id="f64ce-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f64ce-117">Application</span></span>|<span data-ttu-id="f64ce-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f64ce-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f64ce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f64ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}
```

## <a name="request-headers"></a><span data-ttu-id="f64ce-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f64ce-120">Request headers</span></span>
|<span data-ttu-id="f64ce-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f64ce-121">Header</span></span>|<span data-ttu-id="f64ce-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f64ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f64ce-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f64ce-123">Authorization</span></span>|<span data-ttu-id="f64ce-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f64ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f64ce-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f64ce-125">Accept</span></span>|<span data-ttu-id="f64ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f64ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f64ce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f64ce-127">Request body</span></span>
<span data-ttu-id="f64ce-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="f64ce-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object.</span></span>

<span data-ttu-id="f64ce-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md).</span><span class="sxs-lookup"><span data-stu-id="f64ce-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md).</span></span>

|<span data-ttu-id="f64ce-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f64ce-130">Property</span></span>|<span data-ttu-id="f64ce-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f64ce-131">Type</span></span>|<span data-ttu-id="f64ce-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f64ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f64ce-133">id</span><span class="sxs-lookup"><span data-stu-id="f64ce-133">id</span></span>|<span data-ttu-id="f64ce-134">String</span><span class="sxs-lookup"><span data-stu-id="f64ce-134">String</span></span>|<span data-ttu-id="f64ce-135">Chave dessa configuração dentro da política que a contém.</span><span class="sxs-lookup"><span data-stu-id="f64ce-135">Key of this setting within the policy which contains it.</span></span> <span data-ttu-id="f64ce-136">Gerado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="f64ce-136">Automatically generated.</span></span>|
|<span data-ttu-id="f64ce-137">settingInstance</span><span class="sxs-lookup"><span data-stu-id="f64ce-137">settingInstance</span></span>|[<span data-ttu-id="f64ce-138">deviceManagementConfigurationSettingInstance</span><span class="sxs-lookup"><span data-stu-id="f64ce-138">deviceManagementConfigurationSettingInstance</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|<span data-ttu-id="f64ce-139">Instância de configuração</span><span class="sxs-lookup"><span data-stu-id="f64ce-139">Setting Instance</span></span>|



## <a name="response"></a><span data-ttu-id="f64ce-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f64ce-140">Response</span></span>
<span data-ttu-id="f64ce-141">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f64ce-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f64ce-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f64ce-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="f64ce-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f64ce-143">Request</span></span>
<span data-ttu-id="f64ce-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f64ce-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}
Content-type: application/json
Content-length: 7689

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSetting",
  "settingInstance": {
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
                                                                  "children": [
                                                                    {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                      "settingDefinitionId": null,
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

### <a name="response"></a><span data-ttu-id="f64ce-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f64ce-145">Response</span></span>
<span data-ttu-id="f64ce-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f64ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7738

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSetting",
  "id": "9acf977e-977e-9acf-7e97-cf9a7e97cf9a",
  "settingInstance": {
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
                                                                  "children": [
                                                                    {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                      "settingDefinitionId": null,
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





---
title: Criar deviceManagementConfigurationSetting
description: Crie um novo objeto deviceManagementConfigurationSetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 402d49658155300021052722e071704e93080a35
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147018"
---
# <a name="create-devicemanagementconfigurationsetting"></a><span data-ttu-id="7a3ec-103">Criar deviceManagementConfigurationSetting</span><span class="sxs-lookup"><span data-stu-id="7a3ec-103">Create deviceManagementConfigurationSetting</span></span>

<span data-ttu-id="7a3ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a3ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a3ec-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7a3ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a3ec-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a3ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a3ec-107">Crie um novo [objeto deviceManagementConfigurationSetting.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)</span><span class="sxs-lookup"><span data-stu-id="7a3ec-107">Create a new [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a3ec-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7a3ec-108">Prerequisites</span></span>
<span data-ttu-id="7a3ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a3ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a3ec-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a3ec-111">Permission type</span></span>|<span data-ttu-id="7a3ec-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a3ec-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a3ec-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a3ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a3ec-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a3ec-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a3ec-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a3ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a3ec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a3ec-116">Not supported.</span></span>|
|<span data-ttu-id="7a3ec-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a3ec-117">Application</span></span>|<span data-ttu-id="7a3ec-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a3ec-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a3ec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a3ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings
```

## <a name="request-headers"></a><span data-ttu-id="7a3ec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a3ec-120">Request headers</span></span>
|<span data-ttu-id="7a3ec-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a3ec-121">Header</span></span>|<span data-ttu-id="7a3ec-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7a3ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a3ec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a3ec-123">Authorization</span></span>|<span data-ttu-id="7a3ec-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a3ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a3ec-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7a3ec-125">Accept</span></span>|<span data-ttu-id="7a3ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a3ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a3ec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a3ec-127">Request body</span></span>
<span data-ttu-id="7a3ec-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementConfigurationSetting.</span><span class="sxs-lookup"><span data-stu-id="7a3ec-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSetting object.</span></span>

<span data-ttu-id="7a3ec-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationSetting.</span><span class="sxs-lookup"><span data-stu-id="7a3ec-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSetting.</span></span>

|<span data-ttu-id="7a3ec-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a3ec-130">Property</span></span>|<span data-ttu-id="7a3ec-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a3ec-131">Type</span></span>|<span data-ttu-id="7a3ec-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a3ec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a3ec-133">id</span><span class="sxs-lookup"><span data-stu-id="7a3ec-133">id</span></span>|<span data-ttu-id="7a3ec-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a3ec-134">String</span></span>|<span data-ttu-id="7a3ec-135">Chave dessa configuração na política que a contém.</span><span class="sxs-lookup"><span data-stu-id="7a3ec-135">Key of this setting within the policy which contains it.</span></span> <span data-ttu-id="7a3ec-136">Gerado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="7a3ec-136">Automatically generated.</span></span>|
|<span data-ttu-id="7a3ec-137">settingInstance</span><span class="sxs-lookup"><span data-stu-id="7a3ec-137">settingInstance</span></span>|[<span data-ttu-id="7a3ec-138">deviceManagementConfigurationSettingInstance</span><span class="sxs-lookup"><span data-stu-id="7a3ec-138">deviceManagementConfigurationSettingInstance</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|<span data-ttu-id="7a3ec-139">Instância de configuração</span><span class="sxs-lookup"><span data-stu-id="7a3ec-139">Setting Instance</span></span>|



## <a name="response"></a><span data-ttu-id="7a3ec-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a3ec-140">Response</span></span>
<span data-ttu-id="7a3ec-141">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a3ec-141">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a3ec-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a3ec-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a3ec-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a3ec-143">Request</span></span>
<span data-ttu-id="7a3ec-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a3ec-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings
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

### <a name="response"></a><span data-ttu-id="7a3ec-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a3ec-145">Response</span></span>
<span data-ttu-id="7a3ec-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a3ec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





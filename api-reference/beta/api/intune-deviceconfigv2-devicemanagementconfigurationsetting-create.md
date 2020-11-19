---
title: Criar deviceManagementConfigurationSetting
description: Criar um novo objeto deviceManagementConfigurationSetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 981e1e22f670bcb3d703b1dd30623ad264c7a8bd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241369"
---
# <a name="create-devicemanagementconfigurationsetting"></a><span data-ttu-id="42f4b-103">Criar deviceManagementConfigurationSetting</span><span class="sxs-lookup"><span data-stu-id="42f4b-103">Create deviceManagementConfigurationSetting</span></span>

<span data-ttu-id="42f4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42f4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42f4b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42f4b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42f4b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42f4b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42f4b-107">Criar um novo objeto [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="42f4b-107">Create a new [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42f4b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42f4b-108">Prerequisites</span></span>
<span data-ttu-id="42f4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42f4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42f4b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42f4b-111">Permission type</span></span>|<span data-ttu-id="42f4b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42f4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42f4b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42f4b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42f4b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42f4b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42f4b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42f4b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42f4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42f4b-116">Not supported.</span></span>|
|<span data-ttu-id="42f4b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42f4b-117">Application</span></span>|<span data-ttu-id="42f4b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42f4b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42f4b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42f4b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings
```

## <a name="request-headers"></a><span data-ttu-id="42f4b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42f4b-120">Request headers</span></span>
|<span data-ttu-id="42f4b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42f4b-121">Header</span></span>|<span data-ttu-id="42f4b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="42f4b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42f4b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="42f4b-123">Authorization</span></span>|<span data-ttu-id="42f4b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42f4b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42f4b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42f4b-125">Accept</span></span>|<span data-ttu-id="42f4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42f4b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42f4b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42f4b-127">Request body</span></span>
<span data-ttu-id="42f4b-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementConfigurationSetting.</span><span class="sxs-lookup"><span data-stu-id="42f4b-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSetting object.</span></span>

<span data-ttu-id="42f4b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationSetting.</span><span class="sxs-lookup"><span data-stu-id="42f4b-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSetting.</span></span>

|<span data-ttu-id="42f4b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42f4b-130">Property</span></span>|<span data-ttu-id="42f4b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="42f4b-131">Type</span></span>|<span data-ttu-id="42f4b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="42f4b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42f4b-133">id</span><span class="sxs-lookup"><span data-stu-id="42f4b-133">id</span></span>|<span data-ttu-id="42f4b-134">String</span><span class="sxs-lookup"><span data-stu-id="42f4b-134">String</span></span>|<span data-ttu-id="42f4b-135">Chave dessa configuração dentro da política que a contém.</span><span class="sxs-lookup"><span data-stu-id="42f4b-135">Key of this setting within the policy which contains it.</span></span> <span data-ttu-id="42f4b-136">Gerado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="42f4b-136">Automatically generated.</span></span>|
|<span data-ttu-id="42f4b-137">settingInstance</span><span class="sxs-lookup"><span data-stu-id="42f4b-137">settingInstance</span></span>|[<span data-ttu-id="42f4b-138">deviceManagementConfigurationSettingInstance</span><span class="sxs-lookup"><span data-stu-id="42f4b-138">deviceManagementConfigurationSettingInstance</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|<span data-ttu-id="42f4b-139">Instância de configuração</span><span class="sxs-lookup"><span data-stu-id="42f4b-139">Setting Instance</span></span>|



## <a name="response"></a><span data-ttu-id="42f4b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="42f4b-140">Response</span></span>
<span data-ttu-id="42f4b-141">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42f4b-141">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42f4b-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42f4b-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="42f4b-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42f4b-143">Request</span></span>
<span data-ttu-id="42f4b-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42f4b-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="42f4b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="42f4b-145">Response</span></span>
<span data-ttu-id="42f4b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42f4b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





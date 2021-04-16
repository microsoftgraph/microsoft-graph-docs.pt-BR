---
title: Criar deviceManagementReusablePolicySetting
description: Crie um novo objeto deviceManagementReusablePolicySetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 146dfbe24f2380f639ec7715c9ab7cb3278191da
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868374"
---
# <a name="create-devicemanagementreusablepolicysetting"></a><span data-ttu-id="78eb7-103">Criar deviceManagementReusablePolicySetting</span><span class="sxs-lookup"><span data-stu-id="78eb7-103">Create deviceManagementReusablePolicySetting</span></span>

<span data-ttu-id="78eb7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78eb7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78eb7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="78eb7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78eb7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78eb7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78eb7-107">Crie um novo [objeto deviceManagementReusablePolicySetting.](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)</span><span class="sxs-lookup"><span data-stu-id="78eb7-107">Create a new [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78eb7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="78eb7-108">Prerequisites</span></span>
<span data-ttu-id="78eb7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78eb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78eb7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78eb7-111">Permission type</span></span>|<span data-ttu-id="78eb7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78eb7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78eb7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78eb7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78eb7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78eb7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="78eb7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78eb7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78eb7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78eb7-116">Not supported.</span></span>|
|<span data-ttu-id="78eb7-117">Application</span><span class="sxs-lookup"><span data-stu-id="78eb7-117">Application</span></span>|<span data-ttu-id="78eb7-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78eb7-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78eb7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78eb7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reusablePolicySettings
```

## <a name="request-headers"></a><span data-ttu-id="78eb7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78eb7-120">Request headers</span></span>
|<span data-ttu-id="78eb7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78eb7-121">Header</span></span>|<span data-ttu-id="78eb7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="78eb7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78eb7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="78eb7-123">Authorization</span></span>|<span data-ttu-id="78eb7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78eb7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78eb7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="78eb7-125">Accept</span></span>|<span data-ttu-id="78eb7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78eb7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78eb7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78eb7-127">Request body</span></span>
<span data-ttu-id="78eb7-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementReusablePolicySetting.</span><span class="sxs-lookup"><span data-stu-id="78eb7-128">In the request body, supply a JSON representation for the deviceManagementReusablePolicySetting object.</span></span>

<span data-ttu-id="78eb7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementReusablePolicySetting.</span><span class="sxs-lookup"><span data-stu-id="78eb7-129">The following table shows the properties that are required when you create the deviceManagementReusablePolicySetting.</span></span>

|<span data-ttu-id="78eb7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78eb7-130">Property</span></span>|<span data-ttu-id="78eb7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="78eb7-131">Type</span></span>|<span data-ttu-id="78eb7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="78eb7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78eb7-133">id</span><span class="sxs-lookup"><span data-stu-id="78eb7-133">id</span></span>|<span data-ttu-id="78eb7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78eb7-134">String</span></span>|<span data-ttu-id="78eb7-135">id de configuração reutilizável gerada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="78eb7-135">system generated reusable setting id.</span></span>|
|<span data-ttu-id="78eb7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="78eb7-136">displayName</span></span>|<span data-ttu-id="78eb7-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78eb7-137">String</span></span>|<span data-ttu-id="78eb7-138">nome de exibição de configuração reutilizável fornecido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="78eb7-138">reusable setting display name supplied by user.</span></span>|
|<span data-ttu-id="78eb7-139">description</span><span class="sxs-lookup"><span data-stu-id="78eb7-139">description</span></span>|<span data-ttu-id="78eb7-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78eb7-140">String</span></span>|<span data-ttu-id="78eb7-141">descrição da configuração reutilizável fornecida pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="78eb7-141">reusable setting description supplied by user.</span></span>|
|<span data-ttu-id="78eb7-142">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="78eb7-142">settingDefinitionId</span></span>|<span data-ttu-id="78eb7-143">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="78eb7-143">String</span></span>|<span data-ttu-id="78eb7-144">id de definição de definição associada a essa configuração reutilizável.</span><span class="sxs-lookup"><span data-stu-id="78eb7-144">setting definition id associated with this reusable setting.</span></span>|
|<span data-ttu-id="78eb7-145">settingInstance</span><span class="sxs-lookup"><span data-stu-id="78eb7-145">settingInstance</span></span>|[<span data-ttu-id="78eb7-146">deviceManagementConfigurationSettingInstance</span><span class="sxs-lookup"><span data-stu-id="78eb7-146">deviceManagementConfigurationSettingInstance</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|<span data-ttu-id="78eb7-147">instância de configuração de configuração reutilizável</span><span class="sxs-lookup"><span data-stu-id="78eb7-147">reusable setting configuration instance</span></span>|
|<span data-ttu-id="78eb7-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78eb7-148">createdDateTime</span></span>|<span data-ttu-id="78eb7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78eb7-149">DateTimeOffset</span></span>|<span data-ttu-id="78eb7-150">reutilizável definindo data e hora de criação.</span><span class="sxs-lookup"><span data-stu-id="78eb7-150">reusable setting creation date and time.</span></span> <span data-ttu-id="78eb7-151">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78eb7-151">This property is read-only.</span></span>|
|<span data-ttu-id="78eb7-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78eb7-152">lastModifiedDateTime</span></span>|<span data-ttu-id="78eb7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78eb7-153">DateTimeOffset</span></span>|<span data-ttu-id="78eb7-154">data e hora em que a configuração reutilizável foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="78eb7-154">date and time when reusable setting was last modified.</span></span> <span data-ttu-id="78eb7-155">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78eb7-155">This property is read-only.</span></span>|
|<span data-ttu-id="78eb7-156">versão</span><span class="sxs-lookup"><span data-stu-id="78eb7-156">version</span></span>|<span data-ttu-id="78eb7-157">Int32</span><span class="sxs-lookup"><span data-stu-id="78eb7-157">Int32</span></span>|<span data-ttu-id="78eb7-158">número de versão para configuração reutilizável.</span><span class="sxs-lookup"><span data-stu-id="78eb7-158">version number for reusable setting.</span></span> <span data-ttu-id="78eb7-159">Valores válidos de 0 a 2147483647.</span><span class="sxs-lookup"><span data-stu-id="78eb7-159">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="78eb7-160">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78eb7-160">This property is read-only.</span></span>|
|<span data-ttu-id="78eb7-161">referencingConfigurationPolicyCount</span><span class="sxs-lookup"><span data-stu-id="78eb7-161">referencingConfigurationPolicyCount</span></span>|<span data-ttu-id="78eb7-162">Int32</span><span class="sxs-lookup"><span data-stu-id="78eb7-162">Int32</span></span>|<span data-ttu-id="78eb7-163">contagem de políticas de configuração fazendo referência à configuração atual reutilizável.</span><span class="sxs-lookup"><span data-stu-id="78eb7-163">count of configuration policies referencing the current reusable setting.</span></span> <span data-ttu-id="78eb7-164">Valores válidos de 0 a 2147483647.</span><span class="sxs-lookup"><span data-stu-id="78eb7-164">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="78eb7-165">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78eb7-165">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="78eb7-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="78eb7-166">Response</span></span>
<span data-ttu-id="78eb7-167">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78eb7-167">If successful, this method returns a `201 Created` response code and a [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78eb7-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78eb7-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="78eb7-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78eb7-169">Request</span></span>
<span data-ttu-id="78eb7-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78eb7-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reusablePolicySettings
Content-type: application/json
Content-length: 7888

{
  "@odata.type": "#microsoft.graph.deviceManagementReusablePolicySetting",
  "displayName": "Display Name value",
  "description": "Description value",
  "settingDefinitionId": "Setting Definition Id value",
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
  },
  "version": 7,
  "referencingConfigurationPolicyCount": 3
}
```

### <a name="response"></a><span data-ttu-id="78eb7-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="78eb7-171">Response</span></span>
<span data-ttu-id="78eb7-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78eb7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 8060

{
  "@odata.type": "#microsoft.graph.deviceManagementReusablePolicySetting",
  "id": "7a4f9bd7-9bd7-7a4f-d79b-4f7ad79b4f7a",
  "displayName": "Display Name value",
  "description": "Description value",
  "settingDefinitionId": "Setting Definition Id value",
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
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "referencingConfigurationPolicyCount": 3
}
```





---
title: ação clone
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1170cb9aa5854b1f4548b69c38252793fc05324b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868346"
---
# <a name="clone-action"></a><span data-ttu-id="bc158-103">ação clone</span><span class="sxs-lookup"><span data-stu-id="bc158-103">clone action</span></span>

<span data-ttu-id="bc158-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc158-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc158-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc158-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc158-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc158-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc158-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bc158-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc158-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc158-108">Prerequisites</span></span>
<span data-ttu-id="bc158-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc158-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc158-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc158-111">Permission type</span></span>|<span data-ttu-id="bc158-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc158-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc158-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc158-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc158-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc158-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc158-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc158-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc158-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc158-116">Not supported.</span></span>|
|<span data-ttu-id="bc158-117">Application</span><span class="sxs-lookup"><span data-stu-id="bc158-117">Application</span></span>|<span data-ttu-id="bc158-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc158-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc158-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc158-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}/clone
```

## <a name="request-headers"></a><span data-ttu-id="bc158-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc158-120">Request headers</span></span>
|<span data-ttu-id="bc158-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc158-121">Header</span></span>|<span data-ttu-id="bc158-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bc158-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc158-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc158-123">Authorization</span></span>|<span data-ttu-id="bc158-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc158-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc158-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc158-125">Accept</span></span>|<span data-ttu-id="bc158-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc158-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc158-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc158-127">Request body</span></span>
<span data-ttu-id="bc158-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc158-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc158-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc158-129">Response</span></span>
<span data-ttu-id="bc158-130">Se tiver êxito, essa ação retornará um código de resposta e `200 OK` um [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc158-130">If successful, this action returns a `200 OK` response code and a [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc158-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc158-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc158-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc158-132">Request</span></span>
<span data-ttu-id="bc158-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc158-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}/clone
```

### <a name="response"></a><span data-ttu-id="bc158-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc158-134">Response</span></span>
<span data-ttu-id="bc158-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc158-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8302

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
}
```





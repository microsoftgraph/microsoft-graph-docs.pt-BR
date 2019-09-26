---
title: Listar windowsIdentityProtectionConfigurations
description: Listar Propriedades e relações dos objetos windowsIdentityProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0785692210ac4af0ddd79a2ae681ba5b63219174
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37181802"
---
# <a name="list-windowsidentityprotectionconfigurations"></a><span data-ttu-id="b4c2e-103">Listar windowsIdentityProtectionConfigurations</span><span class="sxs-lookup"><span data-stu-id="b4c2e-103">List windowsIdentityProtectionConfigurations</span></span>

> <span data-ttu-id="b4c2e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b4c2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4c2e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4c2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4c2e-106">Listar Propriedades e relações dos objetos [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b4c2e-106">List properties and relationships of the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4c2e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b4c2e-107">Prerequisites</span></span>
<span data-ttu-id="b4c2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4c2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4c2e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4c2e-110">Permission type</span></span>|<span data-ttu-id="b4c2e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b4c2e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4c2e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4c2e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b4c2e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4c2e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b4c2e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4c2e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4c2e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4c2e-115">Not supported.</span></span>|
|<span data-ttu-id="b4c2e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4c2e-116">Application</span></span>|<span data-ttu-id="b4c2e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4c2e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4c2e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4c2e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b4c2e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4c2e-119">Request headers</span></span>
|<span data-ttu-id="b4c2e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4c2e-120">Header</span></span>|<span data-ttu-id="b4c2e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b4c2e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4c2e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4c2e-122">Authorization</span></span>|<span data-ttu-id="b4c2e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4c2e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4c2e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b4c2e-124">Accept</span></span>|<span data-ttu-id="b4c2e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b4c2e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4c2e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4c2e-126">Request body</span></span>
<span data-ttu-id="b4c2e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b4c2e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4c2e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4c2e-128">Response</span></span>
<span data-ttu-id="b4c2e-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4c2e-129">If successful, this method returns a `200 OK` response code and a collection of [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4c2e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4c2e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4c2e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4c2e-131">Request</span></span>
<span data-ttu-id="b4c2e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4c2e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b4c2e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4c2e-133">Response</span></span>
<span data-ttu-id="b4c2e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4c2e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1972

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
      "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "windows10EnterpriseN"
        ],
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "sModeConfiguration",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "useSecurityKeyForSignin": true,
      "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
      "pinMinimumLength": 0,
      "pinMaximumLength": 0,
      "pinUppercaseCharactersUsage": "required",
      "pinLowercaseCharactersUsage": "required",
      "pinSpecialCharactersUsage": "required",
      "pinExpirationInDays": 3,
      "pinPreviousBlockCount": 5,
      "pinRecoveryEnabled": true,
      "securityDeviceRequired": true,
      "unlockWithBiometricsEnabled": true,
      "useCertificatesForOnPremisesAuthEnabled": true,
      "windowsHelloForBusinessBlocked": true
    }
  ]
}
```





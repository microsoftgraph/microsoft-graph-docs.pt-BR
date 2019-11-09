---
title: Obter windowsIdentityProtectionConfiguration
description: Leia as propriedades e as relações do objeto windowsIdentityProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ee3293e15a6b80b328cc86c046ae56a9c8b41d39
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38081643"
---
# <a name="get-windowsidentityprotectionconfiguration"></a><span data-ttu-id="655fd-103">Obter windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="655fd-103">Get windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="655fd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="655fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="655fd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="655fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="655fd-106">Leia as propriedades e as relações do objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="655fd-106">Read properties and relationships of the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="655fd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="655fd-107">Prerequisites</span></span>
<span data-ttu-id="655fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="655fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="655fd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="655fd-110">Permission type</span></span>|<span data-ttu-id="655fd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="655fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="655fd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="655fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="655fd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="655fd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="655fd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="655fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="655fd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="655fd-115">Not supported.</span></span>|
|<span data-ttu-id="655fd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="655fd-116">Application</span></span>|<span data-ttu-id="655fd-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="655fd-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="655fd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="655fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="655fd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="655fd-119">Optional query parameters</span></span>
<span data-ttu-id="655fd-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="655fd-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="655fd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="655fd-121">Request headers</span></span>
|<span data-ttu-id="655fd-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="655fd-122">Header</span></span>|<span data-ttu-id="655fd-123">Valor</span><span class="sxs-lookup"><span data-stu-id="655fd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="655fd-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="655fd-124">Authorization</span></span>|<span data-ttu-id="655fd-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="655fd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="655fd-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="655fd-126">Accept</span></span>|<span data-ttu-id="655fd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="655fd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="655fd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="655fd-128">Request body</span></span>
<span data-ttu-id="655fd-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="655fd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="655fd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="655fd-130">Response</span></span>
<span data-ttu-id="655fd-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="655fd-131">If successful, this method returns a `200 OK` response code and [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="655fd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="655fd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="655fd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="655fd-133">Request</span></span>
<span data-ttu-id="655fd-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="655fd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="655fd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="655fd-135">Response</span></span>
<span data-ttu-id="655fd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="655fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1866

{
  "value": {
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
}
```







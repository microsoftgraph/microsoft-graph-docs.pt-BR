---
title: Listar windowsDefenderAdvancedThreatProtectionConfigurations
description: Listar propriedades e relações dos objetos windowsDefenderAdvancedThreatProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8c63c298f4276145f515ac8348732b8c33152bb5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36314025"
---
# <a name="list-windowsdefenderadvancedthreatprotectionconfigurations"></a><span data-ttu-id="e7971-103">Listar windowsDefenderAdvancedThreatProtectionConfigurations</span><span class="sxs-lookup"><span data-stu-id="e7971-103">List windowsDefenderAdvancedThreatProtectionConfigurations</span></span>

> <span data-ttu-id="e7971-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7971-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7971-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7971-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7971-106">Listar propriedades e relações dos objetos [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7971-106">List properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7971-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7971-107">Prerequisites</span></span>
<span data-ttu-id="e7971-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7971-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7971-110">Permission type</span></span>|<span data-ttu-id="e7971-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7971-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7971-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7971-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7971-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7971-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e7971-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7971-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7971-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7971-115">Not supported.</span></span>|
|<span data-ttu-id="e7971-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7971-116">Application</span></span>|<span data-ttu-id="e7971-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7971-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7971-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7971-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e7971-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7971-119">Request headers</span></span>
|<span data-ttu-id="e7971-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7971-120">Header</span></span>|<span data-ttu-id="e7971-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e7971-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7971-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7971-122">Authorization</span></span>|<span data-ttu-id="e7971-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7971-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7971-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7971-124">Accept</span></span>|<span data-ttu-id="e7971-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7971-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7971-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7971-126">Request body</span></span>
<span data-ttu-id="e7971-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7971-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7971-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7971-128">Response</span></span>
<span data-ttu-id="e7971-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7971-129">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7971-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7971-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7971-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7971-131">Request</span></span>
<span data-ttu-id="e7971-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7971-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="e7971-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7971-133">Response</span></span>
<span data-ttu-id="e7971-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7971-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1964

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
      "id": "294373aa-73aa-2943-aa73-4329aa734329",
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
      "advancedThreatProtectionOnboardingBlob": "Advanced Threat Protection Onboarding Blob value",
      "advancedThreatProtectionOnboardingFilename": "Advanced Threat Protection Onboarding Filename value",
      "advancedThreatProtectionAutoPopulateOnboardingBlob": true,
      "allowSampleSharing": true,
      "enableExpeditedTelemetryReporting": true,
      "advancedThreatProtectionOffboardingBlob": "Advanced Threat Protection Offboarding Blob value",
      "advancedThreatProtectionOffboardingFilename": "Advanced Threat Protection Offboarding Filename value"
    }
  ]
}
```







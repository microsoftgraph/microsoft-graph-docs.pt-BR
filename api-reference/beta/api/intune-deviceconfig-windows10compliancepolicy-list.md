---
title: Listar windows10CompliancePolicies
description: Listar propriedades e relações dos objetos windows10CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 931b7b566968929fa0fe7897eb202fd002ca3731
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48065645"
---
# <a name="list-windows10compliancepolicies"></a><span data-ttu-id="dcffb-103">Listar windows10CompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="dcffb-103">List windows10CompliancePolicies</span></span>

<span data-ttu-id="dcffb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcffb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dcffb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dcffb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcffb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dcffb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcffb-107">Listar propriedades e relações dos objetos [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dcffb-107">List properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcffb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dcffb-108">Prerequisites</span></span>
<span data-ttu-id="dcffb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcffb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcffb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcffb-111">Permission type</span></span>|<span data-ttu-id="dcffb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dcffb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcffb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcffb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dcffb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcffb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dcffb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcffb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcffb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcffb-116">Not supported.</span></span>|
|<span data-ttu-id="dcffb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcffb-117">Application</span></span>|<span data-ttu-id="dcffb-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcffb-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcffb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcffb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="dcffb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcffb-120">Request headers</span></span>
|<span data-ttu-id="dcffb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dcffb-121">Header</span></span>|<span data-ttu-id="dcffb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dcffb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcffb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcffb-123">Authorization</span></span>|<span data-ttu-id="dcffb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcffb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcffb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dcffb-125">Accept</span></span>|<span data-ttu-id="dcffb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dcffb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcffb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcffb-127">Request body</span></span>
<span data-ttu-id="dcffb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dcffb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcffb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcffb-129">Response</span></span>
<span data-ttu-id="dcffb-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcffb-130">If successful, this method returns a `200 OK` response code and a collection of [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcffb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dcffb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcffb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcffb-132">Request</span></span>
<span data-ttu-id="dcffb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcffb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="dcffb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcffb-134">Response</span></span>
<span data-ttu-id="dcffb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dcffb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2328

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "2919ae62-ae62-2919-62ae-192962ae1929",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordRequiredToUnlockFromIdle": true,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "requireHealthyDeviceReport": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
      "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
      "earlyLaunchAntiMalwareDriverEnabled": true,
      "bitLockerEnabled": true,
      "secureBootEnabled": true,
      "codeIntegrityEnabled": true,
      "storageRequireEncryption": true,
      "activeFirewallRequired": true,
      "defenderEnabled": true,
      "defenderVersion": "Defender Version value",
      "signatureOutOfDate": true,
      "rtpEnabled": true,
      "antivirusRequired": true,
      "antiSpywareRequired": true,
      "validOperatingSystemBuildRanges": [
        {
          "@odata.type": "microsoft.graph.operatingSystemVersionRange",
          "description": "Description value",
          "lowestVersion": "Lowest Version value",
          "highestVersion": "Highest Version value"
        }
      ],
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "configurationManagerComplianceRequired": true,
      "tpmRequired": true,
      "deviceCompliancePolicyScript": {
        "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
        "deviceComplianceScriptId": "Device Compliance Script Id value",
        "rulesContent": "cnVsZXNDb250ZW50"
      }
    }
  ]
}
```







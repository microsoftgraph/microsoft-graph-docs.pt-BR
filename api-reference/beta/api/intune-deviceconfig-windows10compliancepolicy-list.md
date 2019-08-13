---
title: Listar windows10CompliancePolicies
description: Listar propriedades e relações dos objetos windows10CompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 365fbee15aa00e0bfb44d7eba0ef56cf2dd59c5a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338501"
---
# <a name="list-windows10compliancepolicies"></a><span data-ttu-id="c0894-103">Listar windows10CompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="c0894-103">List windows10CompliancePolicies</span></span>

> <span data-ttu-id="c0894-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0894-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0894-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0894-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0894-106">Listar propriedades e relações dos objetos [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c0894-106">List properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0894-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0894-107">Prerequisites</span></span>
<span data-ttu-id="c0894-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0894-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0894-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0894-110">Permission type</span></span>|<span data-ttu-id="c0894-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c0894-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0894-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0894-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0894-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0894-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c0894-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0894-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0894-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0894-115">Not supported.</span></span>|
|<span data-ttu-id="c0894-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0894-116">Application</span></span>|<span data-ttu-id="c0894-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0894-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0894-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0894-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="c0894-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0894-119">Request headers</span></span>
|<span data-ttu-id="c0894-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0894-120">Header</span></span>|<span data-ttu-id="c0894-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c0894-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0894-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0894-122">Authorization</span></span>|<span data-ttu-id="c0894-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0894-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0894-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c0894-124">Accept</span></span>|<span data-ttu-id="c0894-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0894-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0894-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0894-126">Request body</span></span>
<span data-ttu-id="c0894-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0894-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0894-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0894-128">Response</span></span>
<span data-ttu-id="c0894-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0894-129">If successful, this method returns a `200 OK` response code and a collection of [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0894-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0894-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0894-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0894-131">Request</span></span>
<span data-ttu-id="c0894-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0894-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="c0894-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0894-133">Response</span></span>
<span data-ttu-id="c0894-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0894-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2087

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
      "tpmRequired": true
    }
  ]
}
```







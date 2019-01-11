---
title: Lista androidWorkProfileCompliancePolicies
description: Lista as propriedades e os relacionamentos dos objetos androidWorkProfileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 43b4959d3d32535d9e8e22dd9ea5a3dc07a0ca1f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856746"
---
# <a name="list-androidworkprofilecompliancepolicies"></a><span data-ttu-id="2d956-103">Lista androidWorkProfileCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="2d956-103">List androidWorkProfileCompliancePolicies</span></span>

> <span data-ttu-id="2d956-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2d956-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d956-105">Lista as propriedades e os relacionamentos dos objetos [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="2d956-105">List properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2d956-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d956-106">Prerequisites</span></span>
<span data-ttu-id="2d956-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d956-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d956-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d956-109">Permission type</span></span>|<span data-ttu-id="2d956-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2d956-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d956-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d956-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2d956-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d956-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2d956-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d956-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d956-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d956-114">Not supported.</span></span>|
|<span data-ttu-id="2d956-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d956-115">Application</span></span>|<span data-ttu-id="2d956-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d956-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d956-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d956-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="2d956-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d956-118">Request headers</span></span>
|<span data-ttu-id="2d956-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d956-119">Header</span></span>|<span data-ttu-id="2d956-120">Valor</span><span class="sxs-lookup"><span data-stu-id="2d956-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d956-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d956-121">Authorization</span></span>|<span data-ttu-id="2d956-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d956-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d956-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2d956-123">Accept</span></span>|<span data-ttu-id="2d956-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2d956-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d956-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d956-125">Request body</span></span>
<span data-ttu-id="2d956-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2d956-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d956-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d956-127">Response</span></span>
<span data-ttu-id="2d956-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d956-128">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d956-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d956-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2d956-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d956-130">Request</span></span>
<span data-ttu-id="2d956-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d956-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="2d956-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d956-132">Response</span></span>
<span data-ttu-id="2d956-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d956-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1487

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
      "id": "4e385271-5271-4e38-7152-384e7152384e",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordMinimumLength": 5,
      "passwordRequiredType": "alphabetic",
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordPreviousPasswordBlockCount": 2,
      "securityPreventInstallAppsFromUnknownSources": true,
      "securityDisableUsbDebugging": true,
      "securityRequireVerifyApps": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "securityBlockJailbrokenDevices": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
      "storageRequireEncryption": true,
      "securityRequireSafetyNetAttestationBasicIntegrity": true,
      "securityRequireSafetyNetAttestationCertifiedDevice": true,
      "securityRequireGooglePlayServices": true,
      "securityRequireUpToDateSecurityProviders": true,
      "securityRequireCompanyPortalAppIntegrity": true
    }
  ]
}
```




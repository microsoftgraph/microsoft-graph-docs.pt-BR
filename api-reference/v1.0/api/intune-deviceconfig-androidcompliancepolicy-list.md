---
title: Listar androidCompliancePolicies
description: Listar propriedades e relações dos objetos androidCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 8d231c2578ebeb3a88372dbc765806a67bdeff3c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313703"
---
# <a name="list-androidcompliancepolicies"></a><span data-ttu-id="5e779-103">Listar androidCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="5e779-103">List androidCompliancePolicies</span></span>

> <span data-ttu-id="5e779-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5e779-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e779-105">Listar propriedades e relações dos objetos [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5e779-105">List properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5e779-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e779-106">Prerequisites</span></span>
<span data-ttu-id="5e779-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e779-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e779-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e779-109">Permission type</span></span>|<span data-ttu-id="5e779-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5e779-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e779-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e779-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5e779-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e779-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5e779-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e779-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e779-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e779-114">Not supported.</span></span>|
|<span data-ttu-id="5e779-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e779-115">Application</span></span>|<span data-ttu-id="5e779-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e779-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e779-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e779-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="5e779-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e779-118">Request headers</span></span>
|<span data-ttu-id="5e779-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e779-119">Header</span></span>|<span data-ttu-id="5e779-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5e779-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e779-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e779-121">Authorization</span></span>|<span data-ttu-id="5e779-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e779-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e779-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5e779-123">Accept</span></span>|<span data-ttu-id="5e779-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5e779-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e779-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e779-125">Request body</span></span>
<span data-ttu-id="5e779-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5e779-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e779-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e779-127">Response</span></span>
<span data-ttu-id="5e779-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e779-128">If successful, this method returns a `200 OK` response code and a collection of [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e779-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e779-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="5e779-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e779-130">Request</span></span>
<span data-ttu-id="5e779-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e779-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="5e779-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e779-132">Response</span></span>
<span data-ttu-id="5e779-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e779-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1476

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidCompliancePolicy",
      "id": "752c820f-820f-752c-0f82-2c750f822c75",
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




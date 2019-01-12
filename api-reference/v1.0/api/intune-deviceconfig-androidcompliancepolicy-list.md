---
title: Listar androidCompliancePolicies
description: Listar propriedades e relações dos objetos androidCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8ec45ff0a3c37456df8e33fe445114141c4d8dad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926971"
---
# <a name="list-androidcompliancepolicies"></a><span data-ttu-id="9f374-103">Listar androidCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="9f374-103">List androidCompliancePolicies</span></span>

> <span data-ttu-id="9f374-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9f374-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f374-105">Listar propriedades e relações dos objetos [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9f374-105">List properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f374-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9f374-106">Prerequisites</span></span>
<span data-ttu-id="9f374-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f374-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f374-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f374-109">Permission type</span></span>|<span data-ttu-id="9f374-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9f374-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f374-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f374-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9f374-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f374-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9f374-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f374-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f374-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f374-114">Not supported.</span></span>|
|<span data-ttu-id="9f374-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f374-115">Application</span></span>|<span data-ttu-id="9f374-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f374-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f374-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f374-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="9f374-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f374-118">Request headers</span></span>
|<span data-ttu-id="9f374-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9f374-119">Header</span></span>|<span data-ttu-id="9f374-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9f374-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f374-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f374-121">Authorization</span></span>|<span data-ttu-id="9f374-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f374-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f374-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9f374-123">Accept</span></span>|<span data-ttu-id="9f374-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9f374-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f374-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f374-125">Request body</span></span>
<span data-ttu-id="9f374-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9f374-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f374-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f374-127">Response</span></span>
<span data-ttu-id="9f374-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f374-128">If successful, this method returns a `200 OK` response code and a collection of [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f374-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f374-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f374-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f374-130">Request</span></span>
<span data-ttu-id="9f374-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f374-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="9f374-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f374-132">Response</span></span>
<span data-ttu-id="9f374-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f374-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




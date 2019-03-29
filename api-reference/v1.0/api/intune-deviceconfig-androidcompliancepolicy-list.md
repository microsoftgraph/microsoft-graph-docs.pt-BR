---
title: Listar androidCompliancePolicies
description: Listar propriedades e relações dos objetos androidCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: debd9ee54f2413859efcd27e380db8992fc9637a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982858"
---
# <a name="list-androidcompliancepolicies"></a><span data-ttu-id="72e2f-103">Listar androidCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="72e2f-103">List androidCompliancePolicies</span></span>

> <span data-ttu-id="72e2f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="72e2f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72e2f-105">Listar propriedades e relações dos objetos [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="72e2f-105">List properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72e2f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72e2f-106">Prerequisites</span></span>
<span data-ttu-id="72e2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72e2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72e2f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72e2f-109">Permission type</span></span>|<span data-ttu-id="72e2f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="72e2f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72e2f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72e2f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="72e2f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="72e2f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="72e2f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72e2f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72e2f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72e2f-114">Not supported.</span></span>|
|<span data-ttu-id="72e2f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72e2f-115">Application</span></span>|<span data-ttu-id="72e2f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72e2f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72e2f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72e2f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="72e2f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72e2f-118">Request headers</span></span>
|<span data-ttu-id="72e2f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72e2f-119">Header</span></span>|<span data-ttu-id="72e2f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="72e2f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72e2f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="72e2f-121">Authorization</span></span>|<span data-ttu-id="72e2f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72e2f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72e2f-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="72e2f-123">Accept</span></span>|<span data-ttu-id="72e2f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="72e2f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72e2f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72e2f-125">Request body</span></span>
<span data-ttu-id="72e2f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72e2f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72e2f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="72e2f-127">Response</span></span>
<span data-ttu-id="72e2f-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72e2f-128">If successful, this method returns a `200 OK` response code and a collection of [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72e2f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72e2f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="72e2f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72e2f-130">Request</span></span>
<span data-ttu-id="72e2f-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72e2f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="72e2f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="72e2f-132">Response</span></span>
<span data-ttu-id="72e2f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72e2f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




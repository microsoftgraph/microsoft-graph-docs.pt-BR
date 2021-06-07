---
title: Obter androidWorkProfileCompliancePolicy
description: Leia propriedades e relações do objeto androidWorkProfileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9d5b6e8dca009b664ba40e02a39f3ea665ab07e8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757196"
---
# <a name="get-androidworkprofilecompliancepolicy"></a><span data-ttu-id="a8185-103">Obter androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a8185-103">Get androidWorkProfileCompliancePolicy</span></span>

<span data-ttu-id="a8185-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8185-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8185-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8185-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8185-106">Leia propriedades e relações do [objeto androidWorkProfileCompliancePolicy.](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a8185-106">Read properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8185-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a8185-107">Prerequisites</span></span>
<span data-ttu-id="a8185-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8185-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8185-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8185-110">Permission type</span></span>|<span data-ttu-id="a8185-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8185-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8185-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8185-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8185-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8185-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8185-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8185-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8185-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8185-115">Not supported.</span></span>|
|<span data-ttu-id="a8185-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8185-116">Application</span></span>|<span data-ttu-id="a8185-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8185-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8185-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8185-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8185-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a8185-119">Optional query parameters</span></span>
<span data-ttu-id="a8185-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a8185-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8185-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8185-121">Request headers</span></span>
|<span data-ttu-id="a8185-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8185-122">Header</span></span>|<span data-ttu-id="a8185-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a8185-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8185-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8185-124">Authorization</span></span>|<span data-ttu-id="a8185-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8185-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8185-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a8185-126">Accept</span></span>|<span data-ttu-id="a8185-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a8185-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8185-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8185-128">Request body</span></span>
<span data-ttu-id="a8185-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8185-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8185-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8185-130">Response</span></span>
<span data-ttu-id="a8185-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8185-131">If successful, this method returns a `200 OK` response code and [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8185-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8185-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8185-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8185-133">Request</span></span>
<span data-ttu-id="a8185-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8185-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="a8185-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8185-135">Response</span></span>
<span data-ttu-id="a8185-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8185-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1417

{
  "value": {
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
}
```





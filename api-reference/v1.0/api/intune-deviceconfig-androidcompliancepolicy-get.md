---
title: Get androidCompliancePolicy
description: Ler propriedades e relações do objeto androidCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: a3e9657e472a58a41e335321685c7a6cb7ac8bb9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354303"
---
# <a name="get-androidcompliancepolicy"></a><span data-ttu-id="83a35-103">Get androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="83a35-103">Get androidCompliancePolicy</span></span>

> <span data-ttu-id="83a35-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="83a35-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83a35-105">Ler propriedades e relações do objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="83a35-105">Read properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83a35-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="83a35-106">Prerequisites</span></span>
<span data-ttu-id="83a35-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83a35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83a35-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83a35-109">Permission type</span></span>|<span data-ttu-id="83a35-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="83a35-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83a35-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83a35-111">Delegated (work or school account)</span></span>|<span data-ttu-id="83a35-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="83a35-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="83a35-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83a35-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83a35-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83a35-114">Not supported.</span></span>|
|<span data-ttu-id="83a35-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83a35-115">Application</span></span>|<span data-ttu-id="83a35-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83a35-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83a35-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83a35-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="83a35-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="83a35-118">Optional query parameters</span></span>
<span data-ttu-id="83a35-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="83a35-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="83a35-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83a35-120">Request headers</span></span>
|<span data-ttu-id="83a35-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83a35-121">Header</span></span>|<span data-ttu-id="83a35-122">Valor</span><span class="sxs-lookup"><span data-stu-id="83a35-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83a35-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="83a35-123">Authorization</span></span>|<span data-ttu-id="83a35-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83a35-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83a35-125">Accept</span><span class="sxs-lookup"><span data-stu-id="83a35-125">Accept</span></span>|<span data-ttu-id="83a35-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83a35-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83a35-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83a35-127">Request body</span></span>
<span data-ttu-id="83a35-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83a35-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83a35-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="83a35-129">Response</span></span>
<span data-ttu-id="83a35-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83a35-130">If successful, this method returns a `200 OK` response code and [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83a35-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83a35-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="83a35-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83a35-132">Request</span></span>
<span data-ttu-id="83a35-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83a35-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="83a35-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="83a35-134">Response</span></span>
<span data-ttu-id="83a35-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83a35-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1406

{
  "value": {
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
}
```




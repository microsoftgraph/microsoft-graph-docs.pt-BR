---
title: Obter androidWorkProfileCompliancePolicy
description: Leia as propriedades e os relacionamentos do objeto androidWorkProfileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e83a7e2404b880d7ada68f5e778ba5acc1186e58
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872027"
---
# <a name="get-androidworkprofilecompliancepolicy"></a><span data-ttu-id="c6d6b-103">Obter androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c6d6b-103">Get androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="c6d6b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c6d6b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6d6b-105">Leia as propriedades e os relacionamentos do objeto [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="c6d6b-105">Read properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c6d6b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c6d6b-106">Prerequisites</span></span>
<span data-ttu-id="c6d6b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6d6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6d6b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6d6b-109">Permission type</span></span>|<span data-ttu-id="c6d6b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c6d6b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6d6b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6d6b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c6d6b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6d6b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c6d6b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6d6b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6d6b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6d6b-114">Not supported.</span></span>|
|<span data-ttu-id="c6d6b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6d6b-115">Application</span></span>|<span data-ttu-id="c6d6b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6d6b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6d6b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6d6b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c6d6b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c6d6b-118">Optional query parameters</span></span>
<span data-ttu-id="c6d6b-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c6d6b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c6d6b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6d6b-120">Request headers</span></span>
|<span data-ttu-id="c6d6b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6d6b-121">Header</span></span>|<span data-ttu-id="c6d6b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c6d6b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6d6b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6d6b-123">Authorization</span></span>|<span data-ttu-id="c6d6b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6d6b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6d6b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c6d6b-125">Accept</span></span>|<span data-ttu-id="c6d6b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6d6b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6d6b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6d6b-127">Request body</span></span>
<span data-ttu-id="c6d6b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c6d6b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6d6b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6d6b-129">Response</span></span>
<span data-ttu-id="c6d6b-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6d6b-130">If successful, this method returns a `200 OK` response code and [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6d6b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6d6b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6d6b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6d6b-132">Request</span></span>
<span data-ttu-id="c6d6b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6d6b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="c6d6b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6d6b-134">Response</span></span>
<span data-ttu-id="c6d6b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6d6b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




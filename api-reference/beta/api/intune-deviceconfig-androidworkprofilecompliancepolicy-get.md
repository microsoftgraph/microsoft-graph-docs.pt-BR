---
title: Obter na entidadeandroidworkprofilecompliancepolicy
description: Leia as propriedades e as relações do objeto na entidadeandroidworkprofilecompliancepolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f1ff51799d43d7813360e910914f94f42f4e235e
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38084731"
---
# <a name="get-androidworkprofilecompliancepolicy"></a><span data-ttu-id="f84e6-103">Obter na entidadeandroidworkprofilecompliancepolicy</span><span class="sxs-lookup"><span data-stu-id="f84e6-103">Get androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="f84e6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f84e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f84e6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f84e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f84e6-106">Leia as propriedades e as relações do objeto [na entidadeandroidworkprofilecompliancepolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f84e6-106">Read properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f84e6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f84e6-107">Prerequisites</span></span>
<span data-ttu-id="f84e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f84e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f84e6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f84e6-110">Permission type</span></span>|<span data-ttu-id="f84e6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f84e6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f84e6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f84e6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f84e6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f84e6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f84e6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f84e6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f84e6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f84e6-115">Not supported.</span></span>|
|<span data-ttu-id="f84e6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f84e6-116">Application</span></span>|<span data-ttu-id="f84e6-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f84e6-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f84e6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f84e6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f84e6-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f84e6-119">Optional query parameters</span></span>
<span data-ttu-id="f84e6-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f84e6-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f84e6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f84e6-121">Request headers</span></span>
|<span data-ttu-id="f84e6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f84e6-122">Header</span></span>|<span data-ttu-id="f84e6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f84e6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f84e6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f84e6-124">Authorization</span></span>|<span data-ttu-id="f84e6-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f84e6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f84e6-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f84e6-126">Accept</span></span>|<span data-ttu-id="f84e6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f84e6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f84e6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f84e6-128">Request body</span></span>
<span data-ttu-id="f84e6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f84e6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f84e6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f84e6-130">Response</span></span>
<span data-ttu-id="f84e6-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [na entidadeandroidworkprofilecompliancepolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f84e6-131">If successful, this method returns a `200 OK` response code and [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f84e6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f84e6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f84e6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f84e6-133">Request</span></span>
<span data-ttu-id="f84e6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f84e6-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="f84e6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f84e6-135">Response</span></span>
<span data-ttu-id="f84e6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f84e6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1542

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
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
    "passwordSignInFailureCountBeforeFactoryReset": 12,
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







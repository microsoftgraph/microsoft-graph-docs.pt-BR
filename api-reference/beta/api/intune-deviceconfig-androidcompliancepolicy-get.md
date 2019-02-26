---
title: Get androidCompliancePolicy
description: Ler propriedades e relações do objeto androidCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e459685924336ce87cd153ac8994e06e5fd43a41
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170704"
---
# <a name="get-androidcompliancepolicy"></a><span data-ttu-id="b0a09-103">Get androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b0a09-103">Get androidCompliancePolicy</span></span>

> <span data-ttu-id="b0a09-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0a09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0a09-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0a09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0a09-106">Ler propriedades e relações do objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0a09-106">Read properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0a09-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0a09-107">Prerequisites</span></span>
<span data-ttu-id="b0a09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b0a09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b0a09-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0a09-110">Permission type</span></span>|<span data-ttu-id="b0a09-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0a09-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0a09-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0a09-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0a09-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0a09-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b0a09-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0a09-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0a09-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0a09-115">Not supported.</span></span>|
|<span data-ttu-id="b0a09-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0a09-116">Application</span></span>|<span data-ttu-id="b0a09-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0a09-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0a09-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0a09-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0a09-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b0a09-119">Optional query parameters</span></span>
<span data-ttu-id="b0a09-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b0a09-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0a09-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0a09-121">Request headers</span></span>
|<span data-ttu-id="b0a09-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0a09-122">Header</span></span>|<span data-ttu-id="b0a09-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b0a09-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0a09-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0a09-124">Authorization</span></span>|<span data-ttu-id="b0a09-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0a09-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0a09-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b0a09-126">Accept</span></span>|<span data-ttu-id="b0a09-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b0a09-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0a09-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0a09-128">Request body</span></span>
<span data-ttu-id="b0a09-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b0a09-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0a09-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0a09-130">Response</span></span>
<span data-ttu-id="b0a09-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0a09-131">If successful, this method returns a `200 OK` response code and [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0a09-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0a09-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0a09-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0a09-133">Request</span></span>
<span data-ttu-id="b0a09-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0a09-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="b0a09-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0a09-135">Response</span></span>
<span data-ttu-id="b0a09-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0a09-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1863

{
  "value": {
    "@odata.type": "#microsoft.graph.androidCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
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
    "securityRequireCompanyPortalAppIntegrity": true,
    "conditionStatementId": "Condition Statement Id value",
    "restrictedApps": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ]
  }
}
```





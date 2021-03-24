---
title: Get androidCompliancePolicy
description: Ler propriedades e relações do objeto androidCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 976bbaf180b70872b8f1dc235d06391ea0c89d57
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126770"
---
# <a name="get-androidcompliancepolicy"></a><span data-ttu-id="abdb0-103">Get androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="abdb0-103">Get androidCompliancePolicy</span></span>

<span data-ttu-id="abdb0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abdb0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="abdb0-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="abdb0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abdb0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="abdb0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abdb0-107">Ler propriedades e relações do objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="abdb0-107">Read properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abdb0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abdb0-108">Prerequisites</span></span>
<span data-ttu-id="abdb0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abdb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abdb0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abdb0-111">Permission type</span></span>|<span data-ttu-id="abdb0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="abdb0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abdb0-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abdb0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abdb0-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abdb0-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="abdb0-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abdb0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abdb0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abdb0-116">Not supported.</span></span>|
|<span data-ttu-id="abdb0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abdb0-117">Application</span></span>|<span data-ttu-id="abdb0-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abdb0-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abdb0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abdb0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abdb0-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="abdb0-120">Optional query parameters</span></span>
<span data-ttu-id="abdb0-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="abdb0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="abdb0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abdb0-122">Request headers</span></span>
|<span data-ttu-id="abdb0-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abdb0-123">Header</span></span>|<span data-ttu-id="abdb0-124">Valor</span><span class="sxs-lookup"><span data-stu-id="abdb0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abdb0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="abdb0-125">Authorization</span></span>|<span data-ttu-id="abdb0-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abdb0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abdb0-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="abdb0-127">Accept</span></span>|<span data-ttu-id="abdb0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="abdb0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abdb0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abdb0-129">Request body</span></span>
<span data-ttu-id="abdb0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="abdb0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abdb0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="abdb0-131">Response</span></span>
<span data-ttu-id="abdb0-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abdb0-132">If successful, this method returns a `200 OK` response code and [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abdb0-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abdb0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="abdb0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abdb0-134">Request</span></span>
<span data-ttu-id="abdb0-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abdb0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="abdb0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="abdb0-136">Response</span></span>
<span data-ttu-id="abdb0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abdb0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2031

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
    "requiredPasswordComplexity": "low",
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordExpirationDays": 6,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "securityPreventInstallAppsFromUnknownSources": true,
    "securityDisableUsbDebugging": true,
    "securityRequireVerifyApps": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "advancedThreatProtectionRequiredSecurityLevel": "secured",
    "securityBlockJailbrokenDevices": true,
    "securityBlockDeviceAdministratorManagedDevices": true,
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





---
title: Listar androidCompliancePolicies
description: Listar propriedades e relações dos objetos androidCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3163fab40dd9580b80020617cc8a659675508d0c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759952"
---
# <a name="list-androidcompliancepolicies"></a><span data-ttu-id="f17cb-103">Listar androidCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="f17cb-103">List androidCompliancePolicies</span></span>

> <span data-ttu-id="f17cb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f17cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f17cb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f17cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f17cb-106">Listar propriedades e relações dos objetos [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f17cb-106">List properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f17cb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f17cb-107">Prerequisites</span></span>
<span data-ttu-id="f17cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f17cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f17cb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f17cb-110">Permission type</span></span>|<span data-ttu-id="f17cb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f17cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f17cb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f17cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f17cb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f17cb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f17cb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f17cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f17cb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f17cb-115">Not supported.</span></span>|
|<span data-ttu-id="f17cb-116">Application</span><span class="sxs-lookup"><span data-stu-id="f17cb-116">Application</span></span>|<span data-ttu-id="f17cb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f17cb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f17cb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f17cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f17cb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f17cb-119">Request headers</span></span>
|<span data-ttu-id="f17cb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f17cb-120">Header</span></span>|<span data-ttu-id="f17cb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f17cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f17cb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f17cb-122">Authorization</span></span>|<span data-ttu-id="f17cb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f17cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f17cb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f17cb-124">Accept</span></span>|<span data-ttu-id="f17cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f17cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f17cb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f17cb-126">Request body</span></span>
<span data-ttu-id="f17cb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f17cb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f17cb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f17cb-128">Response</span></span>
<span data-ttu-id="f17cb-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f17cb-129">If successful, this method returns a `200 OK` response code and a collection of [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f17cb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f17cb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f17cb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f17cb-131">Request</span></span>
<span data-ttu-id="f17cb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f17cb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="f17cb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f17cb-133">Response</span></span>
<span data-ttu-id="f17cb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f17cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2091

{
  "value": [
    {
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
  ]
}
```





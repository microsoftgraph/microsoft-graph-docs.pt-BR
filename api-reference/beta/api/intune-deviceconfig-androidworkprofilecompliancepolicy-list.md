---
title: Listar androidWorkProfileCompliancePolicies
description: Listar Propriedades e relações dos objetos na entidadeandroidworkprofilecompliancepolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c39f959af85a2bf385b5dc4bbda0f4f29cb2ac0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449583"
---
# <a name="list-androidworkprofilecompliancepolicies"></a><span data-ttu-id="0cb17-103">Listar androidWorkProfileCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="0cb17-103">List androidWorkProfileCompliancePolicies</span></span>

<span data-ttu-id="0cb17-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0cb17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cb17-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0cb17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cb17-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0cb17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cb17-107">Listar Propriedades e relações dos objetos [na entidadeandroidworkprofilecompliancepolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="0cb17-107">List properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cb17-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0cb17-108">Prerequisites</span></span>
<span data-ttu-id="0cb17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cb17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cb17-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cb17-111">Permission type</span></span>|<span data-ttu-id="0cb17-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0cb17-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cb17-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cb17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0cb17-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cb17-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0cb17-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cb17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cb17-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cb17-116">Not supported.</span></span>|
|<span data-ttu-id="0cb17-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cb17-117">Application</span></span>|<span data-ttu-id="0cb17-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cb17-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cb17-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cb17-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0cb17-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cb17-120">Request headers</span></span>
|<span data-ttu-id="0cb17-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0cb17-121">Header</span></span>|<span data-ttu-id="0cb17-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0cb17-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cb17-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cb17-123">Authorization</span></span>|<span data-ttu-id="0cb17-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0cb17-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cb17-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0cb17-125">Accept</span></span>|<span data-ttu-id="0cb17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0cb17-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cb17-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cb17-127">Request body</span></span>
<span data-ttu-id="0cb17-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0cb17-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cb17-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cb17-129">Response</span></span>
<span data-ttu-id="0cb17-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [na entidadeandroidworkprofilecompliancepolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cb17-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cb17-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cb17-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cb17-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cb17-132">Request</span></span>
<span data-ttu-id="0cb17-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cb17-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="0cb17-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cb17-134">Response</span></span>
<span data-ttu-id="0cb17-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0cb17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1687

{
  "value": [
    {
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
      "advancedThreatProtectionRequiredSecurityLevel": "secured",
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






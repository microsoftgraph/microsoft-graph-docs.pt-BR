---
title: Obter androidForWorkCompliancePolicy
description: Leia as propriedades e os relacionamentos do objeto androidForWorkCompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6af08fc0c9453e2401036c1538b4be44e8d4f891
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413952"
---
# <a name="get-androidforworkcompliancepolicy"></a><span data-ttu-id="fe7e4-103">Obter androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="fe7e4-103">Get androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="fe7e4-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="fe7e4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fe7e4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fe7e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe7e4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="fe7e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe7e4-107">Leia as propriedades e os relacionamentos do objeto [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="fe7e4-107">Read properties and relationships of the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe7e4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fe7e4-108">Prerequisites</span></span>
<span data-ttu-id="fe7e4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe7e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fe7e4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe7e4-111">Permission type</span></span>|<span data-ttu-id="fe7e4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fe7e4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe7e4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe7e4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe7e4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe7e4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fe7e4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe7e4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe7e4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe7e4-116">Not supported.</span></span>|
|<span data-ttu-id="fe7e4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe7e4-117">Application</span></span>|<span data-ttu-id="fe7e4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe7e4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe7e4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe7e4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe7e4-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fe7e4-120">Optional query parameters</span></span>
<span data-ttu-id="fe7e4-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fe7e4-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe7e4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe7e4-122">Request headers</span></span>
|<span data-ttu-id="fe7e4-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe7e4-123">Header</span></span>|<span data-ttu-id="fe7e4-124">Valor</span><span class="sxs-lookup"><span data-stu-id="fe7e4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe7e4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe7e4-125">Authorization</span></span>|<span data-ttu-id="fe7e4-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe7e4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe7e4-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fe7e4-127">Accept</span></span>|<span data-ttu-id="fe7e4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fe7e4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe7e4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe7e4-129">Request body</span></span>
<span data-ttu-id="fe7e4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe7e4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe7e4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe7e4-131">Response</span></span>
<span data-ttu-id="fe7e4-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe7e4-132">If successful, this method returns a `200 OK` response code and [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe7e4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe7e4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe7e4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe7e4-134">Request</span></span>
<span data-ttu-id="fe7e4-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe7e4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="fe7e4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe7e4-136">Response</span></span>
<span data-ttu-id="fe7e4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe7e4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1538

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "a8d667bd-67bd-a8d6-bd67-d6a8bd67d6a8",
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





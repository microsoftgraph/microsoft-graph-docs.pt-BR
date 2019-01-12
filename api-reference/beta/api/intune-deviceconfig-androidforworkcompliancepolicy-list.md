---
title: Lista androidForWorkCompliancePolicies
description: Lista as propriedades e os relacionamentos dos objetos androidForWorkCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b8bae93ccf0dd16c3ca2ac1b8b64d56d1bbd5c80
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915316"
---
# <a name="list-androidforworkcompliancepolicies"></a><span data-ttu-id="f95b9-103">Lista androidForWorkCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="f95b9-103">List androidForWorkCompliancePolicies</span></span>

> <span data-ttu-id="f95b9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f95b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f95b9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f95b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f95b9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f95b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f95b9-107">Lista as propriedades e os relacionamentos dos objetos [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f95b9-107">List properties and relationships of the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f95b9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f95b9-108">Prerequisites</span></span>
<span data-ttu-id="f95b9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f95b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f95b9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f95b9-111">Permission type</span></span>|<span data-ttu-id="f95b9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f95b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f95b9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f95b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f95b9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f95b9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f95b9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f95b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f95b9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f95b9-116">Not supported.</span></span>|
|<span data-ttu-id="f95b9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f95b9-117">Application</span></span>|<span data-ttu-id="f95b9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f95b9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f95b9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f95b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f95b9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f95b9-120">Request headers</span></span>
|<span data-ttu-id="f95b9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f95b9-121">Header</span></span>|<span data-ttu-id="f95b9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f95b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f95b9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f95b9-123">Authorization</span></span>|<span data-ttu-id="f95b9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f95b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f95b9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f95b9-125">Accept</span></span>|<span data-ttu-id="f95b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f95b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f95b9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f95b9-127">Request body</span></span>
<span data-ttu-id="f95b9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f95b9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f95b9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f95b9-129">Response</span></span>
<span data-ttu-id="f95b9-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f95b9-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f95b9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f95b9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f95b9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f95b9-132">Request</span></span>
<span data-ttu-id="f95b9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f95b9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="f95b9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f95b9-134">Response</span></span>
<span data-ttu-id="f95b9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f95b9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1557

{
  "value": [
    {
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






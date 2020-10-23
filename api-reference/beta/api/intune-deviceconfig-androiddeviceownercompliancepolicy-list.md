---
title: Listar androidDeviceOwnerCompliancePolicies
description: Listar Propriedades e relações dos objetos androidDeviceOwnerCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 539f176af3ebeb222303bb091064b208f9eaed35
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733948"
---
# <a name="list-androiddeviceownercompliancepolicies"></a><span data-ttu-id="bbfb8-103">Listar androidDeviceOwnerCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="bbfb8-103">List androidDeviceOwnerCompliancePolicies</span></span>

<span data-ttu-id="bbfb8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbfb8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbfb8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bbfb8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbfb8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bbfb8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbfb8-107">Listar Propriedades e relações dos objetos [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="bbfb8-107">List properties and relationships of the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbfb8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bbfb8-108">Prerequisites</span></span>
<span data-ttu-id="bbfb8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbfb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbfb8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbfb8-111">Permission type</span></span>|<span data-ttu-id="bbfb8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bbfb8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbfb8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbfb8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bbfb8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbfb8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bbfb8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbfb8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbfb8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbfb8-116">Not supported.</span></span>|
|<span data-ttu-id="bbfb8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbfb8-117">Application</span></span>|<span data-ttu-id="bbfb8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbfb8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbfb8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbfb8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="bbfb8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbfb8-120">Request headers</span></span>
|<span data-ttu-id="bbfb8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bbfb8-121">Header</span></span>|<span data-ttu-id="bbfb8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bbfb8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbfb8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbfb8-123">Authorization</span></span>|<span data-ttu-id="bbfb8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbfb8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbfb8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bbfb8-125">Accept</span></span>|<span data-ttu-id="bbfb8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bbfb8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbfb8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbfb8-127">Request body</span></span>
<span data-ttu-id="bbfb8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bbfb8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbfb8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbfb8-129">Response</span></span>
<span data-ttu-id="bbfb8-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbfb8-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbfb8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbfb8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbfb8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbfb8-132">Request</span></span>
<span data-ttu-id="bbfb8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbfb8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="bbfb8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbfb8-134">Response</span></span>
<span data-ttu-id="bbfb8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bbfb8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1552

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "be2464b4-64b4-be24-b464-24beb46424be",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "advancedThreatProtectionRequiredSecurityLevel": "secured",
      "securityRequireSafetyNetAttestationBasicIntegrity": true,
      "securityRequireSafetyNetAttestationCertifiedDevice": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
      "passwordRequired": true,
      "passwordMinimumLength": 5,
      "passwordMinimumLetterCharacters": 15,
      "passwordMinimumLowerCaseCharacters": 2,
      "passwordMinimumNonLetterCharacters": 2,
      "passwordMinimumNumericCharacters": 0,
      "passwordMinimumSymbolCharacters": 15,
      "passwordMinimumUpperCaseCharacters": 2,
      "passwordRequiredType": "required",
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordPreviousPasswordCountToBlock": 4,
      "storageRequireEncryption": true
    }
  ]
}
```






---
title: Listar androidDeviceOwnerCompliancePolicies
description: Listar Propriedades e relações dos objetos androidDeviceOwnerCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9965df8b8da9d06cdab529f2b2a8db5e79a1d365
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759868"
---
# <a name="list-androiddeviceownercompliancepolicies"></a><span data-ttu-id="1ed1b-103">Listar androidDeviceOwnerCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="1ed1b-103">List androidDeviceOwnerCompliancePolicies</span></span>

> <span data-ttu-id="1ed1b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ed1b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ed1b-106">Listar Propriedades e relações dos objetos [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1ed1b-106">List properties and relationships of the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ed1b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1ed1b-107">Prerequisites</span></span>
<span data-ttu-id="1ed1b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ed1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ed1b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ed1b-110">Permission type</span></span>|<span data-ttu-id="1ed1b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1ed1b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ed1b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ed1b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ed1b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ed1b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1ed1b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ed1b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ed1b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-115">Not supported.</span></span>|
|<span data-ttu-id="1ed1b-116">Application</span><span class="sxs-lookup"><span data-stu-id="1ed1b-116">Application</span></span>|<span data-ttu-id="1ed1b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ed1b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ed1b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ed1b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="1ed1b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ed1b-119">Request headers</span></span>
|<span data-ttu-id="1ed1b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ed1b-120">Header</span></span>|<span data-ttu-id="1ed1b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1ed1b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ed1b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ed1b-122">Authorization</span></span>|<span data-ttu-id="1ed1b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ed1b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1ed1b-124">Accept</span></span>|<span data-ttu-id="1ed1b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1ed1b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ed1b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ed1b-126">Request body</span></span>
<span data-ttu-id="1ed1b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ed1b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ed1b-128">Response</span></span>
<span data-ttu-id="1ed1b-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-129">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ed1b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ed1b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ed1b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ed1b-131">Request</span></span>
<span data-ttu-id="1ed1b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="1ed1b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ed1b-133">Response</span></span>
<span data-ttu-id="1ed1b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





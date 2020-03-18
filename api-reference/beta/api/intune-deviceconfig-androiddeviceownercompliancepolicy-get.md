---
title: Obter androidDeviceOwnerCompliancePolicy
description: Leia as propriedades e as relações do objeto androidDeviceOwnerCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4bbeb476db2890f37a109f6c8edfcf8dc037d5be
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759875"
---
# <a name="get-androiddeviceownercompliancepolicy"></a><span data-ttu-id="30688-103">Obter androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="30688-103">Get androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="30688-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="30688-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30688-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30688-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30688-106">Leia as propriedades e as relações do objeto [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="30688-106">Read properties and relationships of the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30688-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30688-107">Prerequisites</span></span>
<span data-ttu-id="30688-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30688-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30688-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30688-110">Permission type</span></span>|<span data-ttu-id="30688-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30688-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30688-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30688-112">Delegated (work or school account)</span></span>|<span data-ttu-id="30688-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="30688-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="30688-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30688-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30688-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30688-115">Not supported.</span></span>|
|<span data-ttu-id="30688-116">Application</span><span class="sxs-lookup"><span data-stu-id="30688-116">Application</span></span>|<span data-ttu-id="30688-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="30688-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30688-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30688-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30688-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="30688-119">Optional query parameters</span></span>
<span data-ttu-id="30688-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="30688-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30688-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30688-121">Request headers</span></span>
|<span data-ttu-id="30688-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30688-122">Header</span></span>|<span data-ttu-id="30688-123">Valor</span><span class="sxs-lookup"><span data-stu-id="30688-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30688-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="30688-124">Authorization</span></span>|<span data-ttu-id="30688-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30688-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30688-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30688-126">Accept</span></span>|<span data-ttu-id="30688-127">application/json</span><span class="sxs-lookup"><span data-stu-id="30688-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30688-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30688-128">Request body</span></span>
<span data-ttu-id="30688-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30688-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30688-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="30688-130">Response</span></span>
<span data-ttu-id="30688-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30688-131">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30688-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30688-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="30688-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30688-133">Request</span></span>
<span data-ttu-id="30688-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30688-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="30688-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="30688-135">Response</span></span>
<span data-ttu-id="30688-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30688-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1476

{
  "value": {
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
}
```





---
title: Acessar windows10CompliancePolicy
description: Leia as propriedades e as relações do objeto windows10CompliancePolicy.
ms.openlocfilehash: 1e9f6910265e9ee89c9f22ab1876408214858dab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035104"
---
# <a name="get-windows10compliancepolicy"></a><span data-ttu-id="767e5-103">Acessar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="767e5-103">Get windows10CompliancePolicy</span></span>

> <span data-ttu-id="767e5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="767e5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="767e5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="767e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="767e5-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="767e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="767e5-107">Leia as propriedades e as relações do objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="767e5-107">Read properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="767e5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="767e5-108">Prerequisites</span></span>
<span data-ttu-id="767e5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="767e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="767e5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="767e5-111">Permission type</span></span>|<span data-ttu-id="767e5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="767e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="767e5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="767e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="767e5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="767e5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="767e5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="767e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="767e5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="767e5-116">Not supported.</span></span>|
|<span data-ttu-id="767e5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="767e5-117">Application</span></span>|<span data-ttu-id="767e5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="767e5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="767e5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="767e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="767e5-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="767e5-120">Optional query parameters</span></span>
<span data-ttu-id="767e5-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="767e5-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="767e5-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="767e5-122">Request headers</span></span>
|<span data-ttu-id="767e5-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="767e5-123">Header</span></span>|<span data-ttu-id="767e5-124">Valor</span><span class="sxs-lookup"><span data-stu-id="767e5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="767e5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="767e5-125">Authorization</span></span>|<span data-ttu-id="767e5-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="767e5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="767e5-127">Accept</span><span class="sxs-lookup"><span data-stu-id="767e5-127">Accept</span></span>|<span data-ttu-id="767e5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="767e5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="767e5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="767e5-129">Request body</span></span>
<span data-ttu-id="767e5-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="767e5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="767e5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="767e5-131">Response</span></span>
<span data-ttu-id="767e5-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="767e5-132">If successful, this method returns a `200 OK` response code and [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="767e5-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="767e5-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="767e5-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="767e5-134">Request</span></span>
<span data-ttu-id="767e5-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="767e5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="767e5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="767e5-136">Response</span></span>
<span data-ttu-id="767e5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="767e5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1951

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "2919ae62-ae62-2919-62ae-192962ae1929",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordRequiredToUnlockFromIdle": true,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "requireHealthyDeviceReport": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
    "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
    "earlyLaunchAntiMalwareDriverEnabled": true,
    "bitLockerEnabled": true,
    "secureBootEnabled": true,
    "codeIntegrityEnabled": true,
    "storageRequireEncryption": true,
    "activeFirewallRequired": true,
    "defenderEnabled": true,
    "defenderVersion": "Defender Version value",
    "signatureOutOfDate": true,
    "rtpEnabled": true,
    "antivirusRequired": true,
    "antiSpywareRequired": true,
    "validOperatingSystemBuildRanges": [
      {
        "@odata.type": "microsoft.graph.operatingSystemVersionRange",
        "description": "Description value",
        "lowestVersion": "Lowest Version value",
        "highestVersion": "Highest Version value"
      }
    ],
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "configurationManagerComplianceRequired": true
  }
}
```






---
title: Acessar iosCompliancePolicy
description: Leia as propriedades e as relações do objeto iosCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 89e0c7c6d121fbc6ef73b84ba644748e79bf46ee
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304106"
---
# <a name="get-ioscompliancepolicy"></a><span data-ttu-id="33b07-103">Acessar iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="33b07-103">Get iosCompliancePolicy</span></span>

> <span data-ttu-id="33b07-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="33b07-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33b07-105">Leia as propriedades e as relações do objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="33b07-105">Read properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33b07-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33b07-106">Prerequisites</span></span>
<span data-ttu-id="33b07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33b07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33b07-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33b07-109">Permission type</span></span>|<span data-ttu-id="33b07-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="33b07-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33b07-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33b07-111">Delegated (work or school account)</span></span>|<span data-ttu-id="33b07-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="33b07-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="33b07-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33b07-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33b07-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33b07-114">Not supported.</span></span>|
|<span data-ttu-id="33b07-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33b07-115">Application</span></span>|<span data-ttu-id="33b07-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33b07-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33b07-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33b07-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33b07-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="33b07-118">Optional query parameters</span></span>
<span data-ttu-id="33b07-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="33b07-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="33b07-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33b07-120">Request headers</span></span>
|<span data-ttu-id="33b07-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33b07-121">Header</span></span>|<span data-ttu-id="33b07-122">Valor</span><span class="sxs-lookup"><span data-stu-id="33b07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33b07-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="33b07-123">Authorization</span></span>|<span data-ttu-id="33b07-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33b07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33b07-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33b07-125">Accept</span></span>|<span data-ttu-id="33b07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33b07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33b07-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33b07-127">Request body</span></span>
<span data-ttu-id="33b07-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="33b07-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33b07-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="33b07-129">Response</span></span>
<span data-ttu-id="33b07-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33b07-130">If successful, this method returns a `200 OK` response code and [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33b07-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33b07-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="33b07-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33b07-132">Request</span></span>
<span data-ttu-id="33b07-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33b07-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="33b07-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="33b07-134">Response</span></span>
<span data-ttu-id="33b07-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33b07-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 978

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCompliancePolicy",
    "id": "4f501351-1351-4f50-5113-504f5113504f",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passcodeBlockSimple": true,
    "passcodeExpirationDays": 6,
    "passcodeMinimumLength": 5,
    "passcodeMinutesOfInactivityBeforeLock": 5,
    "passcodePreviousPasscodeBlockCount": 2,
    "passcodeMinimumCharacterSetCount": 0,
    "passcodeRequiredType": "alphanumeric",
    "passcodeRequired": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "securityBlockJailbrokenDevices": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "managedEmailProfileRequired": true
  }
}
```




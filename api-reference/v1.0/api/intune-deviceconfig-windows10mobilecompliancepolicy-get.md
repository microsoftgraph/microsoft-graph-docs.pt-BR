---
title: Get windows10MobileCompliancePolicy
description: Ler propriedades e relações do objeto windows10MobileCompliancePolicy.
ms.openlocfilehash: 35f37d4df4ea8862b8fb5ec7a3505a95e73cfae8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005496"
---
# <a name="get-windows10mobilecompliancepolicy"></a><span data-ttu-id="7f766-103">Get windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7f766-103">Get windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="7f766-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7f766-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f766-105">Ler propriedades e relações do objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7f766-105">Read properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f766-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7f766-106">Prerequisites</span></span>
<span data-ttu-id="7f766-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f766-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f766-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f766-109">Permission type</span></span>|<span data-ttu-id="7f766-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7f766-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f766-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f766-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7f766-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f766-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7f766-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f766-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f766-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f766-114">Not supported.</span></span>|
|<span data-ttu-id="7f766-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f766-115">Application</span></span>|<span data-ttu-id="7f766-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f766-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f766-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f766-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f766-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7f766-118">Optional query parameters</span></span>
<span data-ttu-id="7f766-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7f766-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7f766-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f766-120">Request headers</span></span>
|<span data-ttu-id="7f766-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7f766-121">Header</span></span>|<span data-ttu-id="7f766-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7f766-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f766-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f766-123">Authorization</span></span>|<span data-ttu-id="7f766-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f766-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f766-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f766-125">Accept</span></span>|<span data-ttu-id="7f766-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f766-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f766-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f766-127">Request body</span></span>
<span data-ttu-id="7f766-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7f766-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f766-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f766-129">Response</span></span>
<span data-ttu-id="7f766-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f766-130">If successful, this method returns a `200 OK` response code and [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f766-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f766-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f766-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f766-132">Request</span></span>
<span data-ttu-id="7f766-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f766-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="7f766-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f766-134">Response</span></span>
<span data-ttu-id="7f766-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f766-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1029

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
    "id": "3d4237b0-37b0-3d42-b037-423db037423d",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordMinimumLength": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "passwordExpirationDays": 6,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordRequireToUnlockFromIdle": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "earlyLaunchAntiMalwareDriverEnabled": true,
    "bitLockerEnabled": true,
    "secureBootEnabled": true,
    "codeIntegrityEnabled": true,
    "storageRequireEncryption": true
  }
}
```




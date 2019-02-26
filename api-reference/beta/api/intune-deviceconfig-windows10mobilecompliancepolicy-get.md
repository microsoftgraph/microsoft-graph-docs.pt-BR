---
title: Get windows10MobileCompliancePolicy
description: Ler propriedades e relações do objeto windows10MobileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4de8ebfe921c7baa2683f5133505fcd73a8b1bb4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145035"
---
# <a name="get-windows10mobilecompliancepolicy"></a><span data-ttu-id="d9b87-103">Get windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d9b87-103">Get windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="d9b87-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9b87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9b87-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9b87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9b87-106">Ler propriedades e relações do objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d9b87-106">Read properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9b87-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9b87-107">Prerequisites</span></span>
<span data-ttu-id="d9b87-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d9b87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d9b87-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9b87-110">Permission type</span></span>|<span data-ttu-id="d9b87-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9b87-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9b87-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9b87-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9b87-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9b87-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d9b87-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9b87-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9b87-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9b87-115">Not supported.</span></span>|
|<span data-ttu-id="d9b87-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9b87-116">Application</span></span>|<span data-ttu-id="d9b87-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9b87-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9b87-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9b87-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9b87-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d9b87-119">Optional query parameters</span></span>
<span data-ttu-id="d9b87-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d9b87-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9b87-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9b87-121">Request headers</span></span>
|<span data-ttu-id="d9b87-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9b87-122">Header</span></span>|<span data-ttu-id="d9b87-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d9b87-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9b87-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9b87-124">Authorization</span></span>|<span data-ttu-id="d9b87-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9b87-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9b87-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9b87-126">Accept</span></span>|<span data-ttu-id="d9b87-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d9b87-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9b87-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9b87-128">Request body</span></span>
<span data-ttu-id="d9b87-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9b87-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9b87-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9b87-130">Response</span></span>
<span data-ttu-id="d9b87-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9b87-131">If successful, this method returns a `200 OK` response code and [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9b87-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9b87-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9b87-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9b87-133">Request</span></span>
<span data-ttu-id="d9b87-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9b87-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="d9b87-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9b87-135">Response</span></span>
<span data-ttu-id="d9b87-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9b87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1419

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
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
    "storageRequireEncryption": true,
    "activeFirewallRequired": true,
    "validOperatingSystemBuildRanges": [
      {
        "@odata.type": "microsoft.graph.operatingSystemVersionRange",
        "description": "Description value",
        "lowestVersion": "Lowest Version value",
        "highestVersion": "Highest Version value"
      }
    ]
  }
}
```





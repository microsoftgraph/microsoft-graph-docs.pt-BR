---
title: Get managedDevice
description: Ler propriedades e relações do objeto managedDevice.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4df99831f2c3ee53580d033be81bc1a4dbe914d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821936"
---
# <a name="get-manageddevice"></a><span data-ttu-id="d1536-103">Get managedDevice</span><span class="sxs-lookup"><span data-stu-id="d1536-103">Get managedDevice</span></span>

> <span data-ttu-id="d1536-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d1536-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1536-105">Ler propriedades e relações do objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d1536-105">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d1536-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d1536-106">Prerequisites</span></span>
<span data-ttu-id="d1536-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1536-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1536-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1536-109">Permission type</span></span>|<span data-ttu-id="d1536-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d1536-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1536-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1536-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d1536-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1536-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d1536-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1536-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1536-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1536-114">Not supported.</span></span>|
|<span data-ttu-id="d1536-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1536-115">Application</span></span>|<span data-ttu-id="d1536-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1536-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1536-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1536-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/managedDevices/{managedDeviceId}
GET /deviceManagement/managedDevices/{managedDeviceId}
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1536-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1536-118">Optional query parameters</span></span>
<span data-ttu-id="d1536-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d1536-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d1536-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1536-120">Request headers</span></span>
|<span data-ttu-id="d1536-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1536-121">Header</span></span>|<span data-ttu-id="d1536-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d1536-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1536-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1536-123">Authorization</span></span>|<span data-ttu-id="d1536-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1536-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1536-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d1536-125">Accept</span></span>|<span data-ttu-id="d1536-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1536-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1536-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1536-127">Request body</span></span>
<span data-ttu-id="d1536-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1536-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1536-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1536-129">Response</span></span>
<span data-ttu-id="d1536-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDevice](../resources/intune-devices-manageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1536-130">If successful, this method returns a `200 OK` response code and [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1536-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1536-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d1536-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1536-132">Request</span></span>
<span data-ttu-id="d1536-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1536-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}
```

### <a name="response"></a><span data-ttu-id="d1536-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1536-134">Response</span></span>
<span data-ttu-id="d1536-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1536-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4920

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDevice",
    "id": "705c034c-034c-705c-4c03-5c704c035c70",
    "userId": "User Id value",
    "deviceName": "Device Name value",
    "managedDeviceOwnerType": "company",
    "deviceActionResults": [
      {
        "@odata.type": "microsoft.graph.deviceActionResult",
        "actionName": "Action Name value",
        "actionState": "pending",
        "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
        "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
      }
    ],
    "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "operatingSystem": "Operating System value",
    "complianceState": "compliant",
    "jailBroken": "Jail Broken value",
    "managementAgent": "mdm",
    "osVersion": "Os Version value",
    "easActivated": true,
    "easDeviceId": "Eas Device Id value",
    "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
    "azureADRegistered": true,
    "deviceEnrollmentType": "userEnrollment",
    "activationLockBypassCode": "Activation Lock Bypass Code value",
    "emailAddress": "Email Address value",
    "azureADDeviceId": "Azure ADDevice Id value",
    "deviceRegistrationState": "registered",
    "deviceCategoryDisplayName": "Device Category Display Name value",
    "isSupervised": true,
    "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
    "exchangeAccessState": "unknown",
    "exchangeAccessStateReason": "unknown",
    "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
    "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
    "isEncrypted": true,
    "userPrincipalName": "User Principal Name value",
    "model": "Model value",
    "manufacturer": "Manufacturer value",
    "imei": "Imei value",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "serialNumber": "Serial Number value",
    "phoneNumber": "Phone Number value",
    "androidSecurityPatchLevel": "Android Security Patch Level value",
    "userDisplayName": "User Display Name value",
    "configurationManagerClientEnabledFeatures": {
      "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
      "inventory": true,
      "modernApps": true,
      "resourceAccess": true,
      "deviceConfiguration": true,
      "compliancePolicy": true,
      "windowsUpdateForBusiness": true
    },
    "wiFiMacAddress": "Wi Fi Mac Address value",
    "deviceHealthAttestationState": {
      "@odata.type": "microsoft.graph.deviceHealthAttestationState",
      "lastUpdateDateTime": "Last Update Date Time value",
      "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
      "deviceHealthAttestationStatus": "Device Health Attestation Status value",
      "contentVersion": "Content Version value",
      "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
      "attestationIdentityKey": "Attestation Identity Key value",
      "resetCount": 10,
      "restartCount": 12,
      "dataExcutionPolicy": "Data Excution Policy value",
      "bitLockerStatus": "Bit Locker Status value",
      "bootManagerVersion": "Boot Manager Version value",
      "codeIntegrityCheckVersion": "Code Integrity Check Version value",
      "secureBoot": "Secure Boot value",
      "bootDebugging": "Boot Debugging value",
      "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
      "codeIntegrity": "Code Integrity value",
      "testSigning": "Test Signing value",
      "safeMode": "Safe Mode value",
      "windowsPE": "Windows PE value",
      "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
      "virtualSecureMode": "Virtual Secure Mode value",
      "pcrHashAlgorithm": "Pcr Hash Algorithm value",
      "bootAppSecurityVersion": "Boot App Security Version value",
      "bootManagerSecurityVersion": "Boot Manager Security Version value",
      "tpmVersion": "Tpm Version value",
      "pcr0": "Pcr0 value",
      "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
      "codeIntegrityPolicy": "Code Integrity Policy value",
      "bootRevisionListInfo": "Boot Revision List Info value",
      "operatingSystemRevListInfo": "Operating System Rev List Info value",
      "healthStatusMismatchInfo": "Health Status Mismatch Info value",
      "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
    },
    "subscriberCarrier": "Subscriber Carrier value",
    "meid": "Meid value",
    "totalStorageSpaceInBytes": 8,
    "freeStorageSpaceInBytes": 7,
    "managedDeviceName": "Managed Device Name value",
    "partnerReportedThreatState": "activated"
  }
}
```




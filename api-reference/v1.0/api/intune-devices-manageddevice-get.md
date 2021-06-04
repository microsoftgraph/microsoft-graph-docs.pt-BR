---
title: Acessar managedDevice
description: Leia as propriedades e as relações do objeto managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d98fdc01f19aa20ae4d5de74b8b4bdcbf8671138
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753684"
---
# <a name="get-manageddevice"></a><span data-ttu-id="06edc-103">Acessar managedDevice</span><span class="sxs-lookup"><span data-stu-id="06edc-103">Get managedDevice</span></span>

<span data-ttu-id="06edc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06edc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06edc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06edc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06edc-106">Leia as propriedades e as relações do objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="06edc-106">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06edc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06edc-107">Prerequisites</span></span>
<span data-ttu-id="06edc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06edc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06edc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06edc-110">Permission type</span></span>|<span data-ttu-id="06edc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06edc-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06edc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06edc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06edc-113">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06edc-113">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="06edc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06edc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06edc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06edc-115">Not supported.</span></span>|
|<span data-ttu-id="06edc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06edc-116">Application</span></span>|<span data-ttu-id="06edc-117">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06edc-117">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06edc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06edc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/managedDevices/{managedDeviceId}
GET /deviceManagement/managedDevices/{managedDeviceId}
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06edc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="06edc-119">Optional query parameters</span></span>
<span data-ttu-id="06edc-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="06edc-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06edc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06edc-121">Request headers</span></span>
|<span data-ttu-id="06edc-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06edc-122">Header</span></span>|<span data-ttu-id="06edc-123">Valor</span><span class="sxs-lookup"><span data-stu-id="06edc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06edc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="06edc-124">Authorization</span></span>|<span data-ttu-id="06edc-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06edc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06edc-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06edc-126">Accept</span></span>|<span data-ttu-id="06edc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="06edc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06edc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06edc-128">Request body</span></span>
<span data-ttu-id="06edc-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06edc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06edc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="06edc-130">Response</span></span>
<span data-ttu-id="06edc-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedDevice](../resources/intune-devices-manageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06edc-131">If successful, this method returns a `200 OK` response code and [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06edc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06edc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="06edc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06edc-133">Request</span></span>
<span data-ttu-id="06edc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06edc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}
```

### <a name="response"></a><span data-ttu-id="06edc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="06edc-135">Response</span></span>
<span data-ttu-id="06edc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06edc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5095

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
    "partnerReportedThreatState": "activated",
    "iccid": "Iccid value",
    "udid": "Udid value",
    "notes": "Notes value",
    "ethernetMacAddress": "Ethernet Mac Address value",
    "physicalMemoryInBytes": 5
  }
}
```





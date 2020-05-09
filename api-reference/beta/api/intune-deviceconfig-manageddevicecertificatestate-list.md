---
title: Listar managedDeviceCertificateStates
description: Listar Propriedades e relações dos objetos managedDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e30b0450f9bbf3893d9d38cba3f97483e8221087
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179120"
---
# <a name="list-manageddevicecertificatestates"></a><span data-ttu-id="160ab-103">Listar managedDeviceCertificateStates</span><span class="sxs-lookup"><span data-stu-id="160ab-103">List managedDeviceCertificateStates</span></span>

<span data-ttu-id="160ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="160ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="160ab-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="160ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="160ab-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="160ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="160ab-107">Listar Propriedades e relações dos objetos [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="160ab-107">List properties and relationships of the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="160ab-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="160ab-108">Prerequisites</span></span>
<span data-ttu-id="160ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="160ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="160ab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="160ab-111">Permission type</span></span>|<span data-ttu-id="160ab-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="160ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="160ab-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="160ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="160ab-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="160ab-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="160ab-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="160ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="160ab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="160ab-116">Not supported.</span></span>|
|<span data-ttu-id="160ab-117">Application</span><span class="sxs-lookup"><span data-stu-id="160ab-117">Application</span></span>|<span data-ttu-id="160ab-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="160ab-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="160ab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="160ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="160ab-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="160ab-120">Request headers</span></span>
|<span data-ttu-id="160ab-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="160ab-121">Header</span></span>|<span data-ttu-id="160ab-122">Valor</span><span class="sxs-lookup"><span data-stu-id="160ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="160ab-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="160ab-123">Authorization</span></span>|<span data-ttu-id="160ab-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="160ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="160ab-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="160ab-125">Accept</span></span>|<span data-ttu-id="160ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="160ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="160ab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="160ab-127">Request body</span></span>
<span data-ttu-id="160ab-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="160ab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="160ab-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="160ab-129">Response</span></span>
<span data-ttu-id="160ab-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="160ab-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="160ab-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="160ab-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="160ab-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="160ab-132">Request</span></span>
<span data-ttu-id="160ab-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="160ab-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
```

### <a name="response"></a><span data-ttu-id="160ab-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="160ab-134">Response</span></span>
<span data-ttu-id="160ab-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="160ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1703

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
      "id": "d99bc884-c884-d99b-84c8-9bd984c89bd9",
      "devicePlatform": "androidForWork",
      "certificateKeyUsage": "digitalSignature",
      "certificateValidityPeriodUnits": "months",
      "certificateIssuanceState": "challengeIssued",
      "certificateKeyStorageProvider": "useTpmKspOtherwiseFail",
      "certificateSubjectNameFormat": "commonNameIncludingEmail",
      "certificateSubjectAlternativeNameFormat": "emailAddress",
      "certificateRevokeStatus": "pending",
      "certificateProfileDisplayName": "Certificate Profile Display Name value",
      "deviceDisplayName": "Device Display Name value",
      "userDisplayName": "User Display Name value",
      "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
      "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:00:27.7468732-08:00",
      "lastCertificateStateChangeDateTime": "2017-01-01T00:01:10.7144639-08:00",
      "certificateIssuer": "Certificate Issuer value",
      "certificateThumbprint": "Certificate Thumbprint value",
      "certificateSerialNumber": "Certificate Serial Number value",
      "certificateKeyLength": 4,
      "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
      "certificateValidityPeriod": 9,
      "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
      "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
      "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
      "certificateErrorCode": 4
    }
  ]
}
```




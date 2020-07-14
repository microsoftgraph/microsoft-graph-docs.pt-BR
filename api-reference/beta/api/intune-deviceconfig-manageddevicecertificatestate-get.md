---
title: Obter managedDeviceCertificateState
description: Leia as propriedades e as relações do objeto managedDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db90ac49069e0a9c971bc0779dd412ce2db042ba
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122865"
---
# <a name="get-manageddevicecertificatestate"></a><span data-ttu-id="55f46-103">Obter managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="55f46-103">Get managedDeviceCertificateState</span></span>

<span data-ttu-id="55f46-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55f46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55f46-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="55f46-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55f46-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55f46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55f46-107">Leia as propriedades e as relações do objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="55f46-107">Read properties and relationships of the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55f46-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="55f46-108">Prerequisites</span></span>
<span data-ttu-id="55f46-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="55f46-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="55f46-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55f46-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55f46-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55f46-111">Permission type</span></span>|<span data-ttu-id="55f46-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55f46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55f46-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55f46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55f46-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="55f46-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="55f46-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55f46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55f46-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55f46-116">Not supported.</span></span>|
|<span data-ttu-id="55f46-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55f46-117">Application</span></span>|<span data-ttu-id="55f46-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="55f46-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55f46-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55f46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55f46-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="55f46-120">Optional query parameters</span></span>
<span data-ttu-id="55f46-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="55f46-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55f46-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55f46-122">Request headers</span></span>
|<span data-ttu-id="55f46-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55f46-123">Header</span></span>|<span data-ttu-id="55f46-124">Valor</span><span class="sxs-lookup"><span data-stu-id="55f46-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55f46-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="55f46-125">Authorization</span></span>|<span data-ttu-id="55f46-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55f46-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55f46-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="55f46-127">Accept</span></span>|<span data-ttu-id="55f46-128">application/json</span><span class="sxs-lookup"><span data-stu-id="55f46-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55f46-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55f46-129">Request body</span></span>
<span data-ttu-id="55f46-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55f46-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55f46-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="55f46-131">Response</span></span>
<span data-ttu-id="55f46-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55f46-132">If successful, this method returns a `200 OK` response code and [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55f46-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55f46-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="55f46-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55f46-134">Request</span></span>
<span data-ttu-id="55f46-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55f46-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="55f46-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="55f46-136">Response</span></span>
<span data-ttu-id="55f46-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="55f46-137">Here is an example of the response.</span></span> <span data-ttu-id="55f46-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="55f46-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="55f46-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="55f46-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1637

{
  "value": {
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
}
```




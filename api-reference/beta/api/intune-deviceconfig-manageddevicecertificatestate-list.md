---
title: Listar managedDeviceCertificateStates
description: Listar propriedades e relações dos objetos managedDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c6026e4d6a4c158ebed2b9a6e7f535ec7406535b
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626008"
---
# <a name="list-manageddevicecertificatestates"></a><span data-ttu-id="f0b70-103">Listar managedDeviceCertificateStates</span><span class="sxs-lookup"><span data-stu-id="f0b70-103">List managedDeviceCertificateStates</span></span>

<span data-ttu-id="f0b70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0b70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0b70-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f0b70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0b70-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0b70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0b70-107">Listar propriedades e relações dos [objetos managedDeviceCertificateState.](../resources/intune-deviceconfig-manageddevicecertificatestate.md)</span><span class="sxs-lookup"><span data-stu-id="f0b70-107">List properties and relationships of the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0b70-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f0b70-108">Prerequisites</span></span>
<span data-ttu-id="f0b70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0b70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0b70-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0b70-111">Permission type</span></span>|<span data-ttu-id="f0b70-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f0b70-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0b70-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0b70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0b70-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0b70-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f0b70-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0b70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0b70-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0b70-116">Not supported.</span></span>|
|<span data-ttu-id="f0b70-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0b70-117">Application</span></span>|<span data-ttu-id="f0b70-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0b70-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0b70-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0b70-119">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="f0b70-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0b70-120">Request headers</span></span>
|<span data-ttu-id="f0b70-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f0b70-121">Header</span></span>|<span data-ttu-id="f0b70-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f0b70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0b70-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0b70-123">Authorization</span></span>|<span data-ttu-id="f0b70-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0b70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0b70-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f0b70-125">Accept</span></span>|<span data-ttu-id="f0b70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0b70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0b70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0b70-127">Request body</span></span>
<span data-ttu-id="f0b70-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0b70-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0b70-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0b70-129">Response</span></span>
<span data-ttu-id="f0b70-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0b70-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0b70-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0b70-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0b70-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0b70-132">Request</span></span>
<span data-ttu-id="f0b70-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0b70-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
```

### <a name="response"></a><span data-ttu-id="f0b70-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0b70-134">Response</span></span>
<span data-ttu-id="f0b70-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0b70-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





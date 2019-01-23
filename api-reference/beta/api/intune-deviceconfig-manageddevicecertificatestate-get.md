---
title: Obter managedDeviceCertificateState
description: Leia as propriedades e os relacionamentos do objeto managedDeviceCertificateState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a38731606957ade6c718b030045b236636f5acbf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403788"
---
# <a name="get-manageddevicecertificatestate"></a><span data-ttu-id="fbb4e-103">Obter managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="fbb4e-103">Get managedDeviceCertificateState</span></span>

> <span data-ttu-id="fbb4e-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="fbb4e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fbb4e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fbb4e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbb4e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="fbb4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbb4e-107">Leia as propriedades e os relacionamentos do objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="fbb4e-107">Read properties and relationships of the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbb4e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbb4e-108">Prerequisites</span></span>
<span data-ttu-id="fbb4e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fbb4e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fbb4e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbb4e-111">Permission type</span></span>|<span data-ttu-id="fbb4e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fbb4e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbb4e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbb4e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbb4e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbb4e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fbb4e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbb4e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbb4e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbb4e-116">Not supported.</span></span>|
|<span data-ttu-id="fbb4e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbb4e-117">Application</span></span>|<span data-ttu-id="fbb4e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbb4e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbb4e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbb4e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fbb4e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fbb4e-120">Optional query parameters</span></span>
<span data-ttu-id="fbb4e-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fbb4e-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fbb4e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbb4e-122">Request headers</span></span>
|<span data-ttu-id="fbb4e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbb4e-123">Header</span></span>|<span data-ttu-id="fbb4e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="fbb4e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbb4e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbb4e-125">Authorization</span></span>|<span data-ttu-id="fbb4e-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbb4e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbb4e-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fbb4e-127">Accept</span></span>|<span data-ttu-id="fbb4e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fbb4e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbb4e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbb4e-129">Request body</span></span>
<span data-ttu-id="fbb4e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fbb4e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbb4e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbb4e-131">Response</span></span>
<span data-ttu-id="fbb4e-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbb4e-132">If successful, this method returns a `200 OK` response code and [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbb4e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbb4e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbb4e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbb4e-134">Request</span></span>
<span data-ttu-id="fbb4e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbb4e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="fbb4e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbb4e-136">Response</span></span>
<span data-ttu-id="fbb4e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbb4e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





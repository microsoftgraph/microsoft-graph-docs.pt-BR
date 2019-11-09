---
title: Obter managedAllDeviceCertificateState
description: Leia as propriedades e as relações do objeto managedAllDeviceCertificateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dcd53efee18eaad354c4313108fd3fed4a1601fa
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38083393"
---
# <a name="get-managedalldevicecertificatestate"></a><span data-ttu-id="6a147-103">Obter managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="6a147-103">Get managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="6a147-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a147-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a147-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a147-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a147-106">Leia as propriedades e as relações do objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="6a147-106">Read properties and relationships of the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a147-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a147-107">Prerequisites</span></span>
<span data-ttu-id="6a147-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a147-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a147-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a147-110">Permission type</span></span>|<span data-ttu-id="6a147-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6a147-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a147-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a147-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a147-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a147-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6a147-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a147-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a147-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a147-115">Not supported.</span></span>|
|<span data-ttu-id="6a147-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a147-116">Application</span></span>|<span data-ttu-id="6a147-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a147-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a147-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a147-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a147-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6a147-119">Optional query parameters</span></span>
<span data-ttu-id="6a147-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6a147-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a147-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a147-121">Request headers</span></span>
|<span data-ttu-id="6a147-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a147-122">Header</span></span>|<span data-ttu-id="6a147-123">Valor</span><span class="sxs-lookup"><span data-stu-id="6a147-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a147-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a147-124">Authorization</span></span>|<span data-ttu-id="6a147-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a147-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a147-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a147-126">Accept</span></span>|<span data-ttu-id="6a147-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6a147-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a147-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a147-128">Request body</span></span>
<span data-ttu-id="6a147-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a147-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a147-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a147-130">Response</span></span>
<span data-ttu-id="6a147-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a147-131">If successful, this method returns a `200 OK` response code and [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a147-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a147-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a147-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a147-133">Request</span></span>
<span data-ttu-id="6a147-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a147-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="6a147-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a147-135">Response</span></span>
<span data-ttu-id="6a147-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a147-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 829

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
    "id": "987c6a17-6a17-987c-176a-7c98176a7c98",
    "certificateRevokeStatus": "pending",
    "managedDeviceDisplayName": "Managed Device Display Name value",
    "userPrincipalName": "User Principal Name value",
    "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
    "certificateIssuerName": "Certificate Issuer Name value",
    "certificateThumbprint": "Certificate Thumbprint value",
    "certificateSerialNumber": "Certificate Serial Number value",
    "certificateSubjectName": "Certificate Subject Name value",
    "certificateKeyUsages": 4,
    "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
    "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00"
  }
}
```







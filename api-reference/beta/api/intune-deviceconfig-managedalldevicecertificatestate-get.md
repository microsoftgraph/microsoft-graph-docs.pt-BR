---
title: Obter managedAllDeviceCertificateState
description: Leia as propriedades e as relações do objeto managedAllDeviceCertificateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ba57a94877db3a94b0021cd931fbeca0896637ec
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345628"
---
# <a name="get-managedalldevicecertificatestate"></a><span data-ttu-id="e772f-103">Obter managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="e772f-103">Get managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="e772f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e772f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e772f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e772f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e772f-106">Leia as propriedades e as relações do objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="e772f-106">Read properties and relationships of the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e772f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e772f-107">Prerequisites</span></span>
<span data-ttu-id="e772f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e772f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e772f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e772f-110">Permission type</span></span>|<span data-ttu-id="e772f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e772f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e772f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e772f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e772f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e772f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e772f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e772f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e772f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e772f-115">Not supported.</span></span>|
|<span data-ttu-id="e772f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e772f-116">Application</span></span>|<span data-ttu-id="e772f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e772f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e772f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e772f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e772f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e772f-119">Optional query parameters</span></span>
<span data-ttu-id="e772f-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e772f-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e772f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e772f-121">Request headers</span></span>
|<span data-ttu-id="e772f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e772f-122">Header</span></span>|<span data-ttu-id="e772f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e772f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e772f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e772f-124">Authorization</span></span>|<span data-ttu-id="e772f-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e772f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e772f-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e772f-126">Accept</span></span>|<span data-ttu-id="e772f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e772f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e772f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e772f-128">Request body</span></span>
<span data-ttu-id="e772f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e772f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e772f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e772f-130">Response</span></span>
<span data-ttu-id="e772f-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e772f-131">If successful, this method returns a `200 OK` response code and [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e772f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e772f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e772f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e772f-133">Request</span></span>
<span data-ttu-id="e772f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e772f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="e772f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e772f-135">Response</span></span>
<span data-ttu-id="e772f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e772f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







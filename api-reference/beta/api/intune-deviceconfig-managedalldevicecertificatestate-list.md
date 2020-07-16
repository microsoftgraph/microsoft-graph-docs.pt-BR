---
title: Listar managedAllDeviceCertificateStates
description: Listar Propriedades e relações dos objetos managedAllDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e255f849d447fb82f5b796cd5262652d0ac2526f
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122942"
---
# <a name="list-managedalldevicecertificatestates"></a><span data-ttu-id="61528-103">Listar managedAllDeviceCertificateStates</span><span class="sxs-lookup"><span data-stu-id="61528-103">List managedAllDeviceCertificateStates</span></span>

<span data-ttu-id="61528-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61528-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61528-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="61528-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61528-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61528-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61528-107">Listar Propriedades e relações dos objetos [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="61528-107">List properties and relationships of the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61528-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61528-108">Prerequisites</span></span>
<span data-ttu-id="61528-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61528-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61528-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61528-111">Permission type</span></span>|<span data-ttu-id="61528-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61528-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61528-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61528-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61528-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="61528-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="61528-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61528-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61528-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61528-116">Not supported.</span></span>|
|<span data-ttu-id="61528-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61528-117">Application</span></span>|<span data-ttu-id="61528-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="61528-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61528-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61528-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="61528-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61528-120">Request headers</span></span>
|<span data-ttu-id="61528-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61528-121">Header</span></span>|<span data-ttu-id="61528-122">Valor</span><span class="sxs-lookup"><span data-stu-id="61528-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61528-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="61528-123">Authorization</span></span>|<span data-ttu-id="61528-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61528-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61528-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61528-125">Accept</span></span>|<span data-ttu-id="61528-126">application/json</span><span class="sxs-lookup"><span data-stu-id="61528-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61528-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61528-127">Request body</span></span>
<span data-ttu-id="61528-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61528-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61528-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="61528-129">Response</span></span>
<span data-ttu-id="61528-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61528-130">If successful, this method returns a `200 OK` response code and a collection of [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61528-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61528-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="61528-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61528-132">Request</span></span>
<span data-ttu-id="61528-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61528-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

### <a name="response"></a><span data-ttu-id="61528-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="61528-134">Response</span></span>
<span data-ttu-id="61528-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61528-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 958

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
      "id": "987c6a17-6a17-987c-176a-7c98176a7c98",
      "certificateRevokeStatus": "pending",
      "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:34.9547208-08:00",
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
  ]
}
```




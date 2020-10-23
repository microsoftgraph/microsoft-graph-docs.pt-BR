---
title: Listar managedAllDeviceCertificateStates
description: Listar Propriedades e relações dos objetos managedAllDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b2c2bb15b6f13125409911b4a15732791623fe86
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693476"
---
# <a name="list-managedalldevicecertificatestates"></a><span data-ttu-id="08c24-103">Listar managedAllDeviceCertificateStates</span><span class="sxs-lookup"><span data-stu-id="08c24-103">List managedAllDeviceCertificateStates</span></span>

<span data-ttu-id="08c24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08c24-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08c24-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="08c24-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08c24-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08c24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08c24-107">Listar Propriedades e relações dos objetos [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="08c24-107">List properties and relationships of the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08c24-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="08c24-108">Prerequisites</span></span>
<span data-ttu-id="08c24-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08c24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08c24-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08c24-111">Permission type</span></span>|<span data-ttu-id="08c24-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="08c24-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08c24-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08c24-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08c24-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="08c24-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="08c24-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08c24-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08c24-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08c24-116">Not supported.</span></span>|
|<span data-ttu-id="08c24-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08c24-117">Application</span></span>|<span data-ttu-id="08c24-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="08c24-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08c24-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08c24-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="08c24-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08c24-120">Request headers</span></span>
|<span data-ttu-id="08c24-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="08c24-121">Header</span></span>|<span data-ttu-id="08c24-122">Valor</span><span class="sxs-lookup"><span data-stu-id="08c24-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08c24-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="08c24-123">Authorization</span></span>|<span data-ttu-id="08c24-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08c24-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08c24-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="08c24-125">Accept</span></span>|<span data-ttu-id="08c24-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08c24-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08c24-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08c24-127">Request body</span></span>
<span data-ttu-id="08c24-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="08c24-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08c24-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="08c24-129">Response</span></span>
<span data-ttu-id="08c24-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08c24-130">If successful, this method returns a `200 OK` response code and a collection of [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08c24-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08c24-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="08c24-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08c24-132">Request</span></span>
<span data-ttu-id="08c24-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08c24-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

### <a name="response"></a><span data-ttu-id="08c24-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="08c24-134">Response</span></span>
<span data-ttu-id="08c24-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08c24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






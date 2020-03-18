---
title: Listar managedAllDeviceCertificateStates
description: Listar Propriedades e relações dos objetos managedAllDeviceCertificateState.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5b13b63b41afa3f630acf1012be0089bcd21fe1a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42743489"
---
# <a name="list-managedalldevicecertificatestates"></a><span data-ttu-id="cb530-103">Listar managedAllDeviceCertificateStates</span><span class="sxs-lookup"><span data-stu-id="cb530-103">List managedAllDeviceCertificateStates</span></span>

> <span data-ttu-id="cb530-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cb530-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb530-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb530-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb530-106">Listar Propriedades e relações dos objetos [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="cb530-106">List properties and relationships of the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb530-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cb530-107">Prerequisites</span></span>
<span data-ttu-id="cb530-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb530-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb530-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb530-110">Permission type</span></span>|<span data-ttu-id="cb530-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cb530-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb530-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb530-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb530-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb530-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cb530-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb530-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb530-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb530-115">Not supported.</span></span>|
|<span data-ttu-id="cb530-116">Application</span><span class="sxs-lookup"><span data-stu-id="cb530-116">Application</span></span>|<span data-ttu-id="cb530-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb530-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb530-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb530-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="cb530-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb530-119">Request headers</span></span>
|<span data-ttu-id="cb530-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb530-120">Header</span></span>|<span data-ttu-id="cb530-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cb530-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb530-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb530-122">Authorization</span></span>|<span data-ttu-id="cb530-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb530-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb530-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cb530-124">Accept</span></span>|<span data-ttu-id="cb530-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cb530-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb530-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb530-126">Request body</span></span>
<span data-ttu-id="cb530-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb530-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb530-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb530-128">Response</span></span>
<span data-ttu-id="cb530-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb530-129">If successful, this method returns a `200 OK` response code and a collection of [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb530-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb530-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb530-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb530-131">Request</span></span>
<span data-ttu-id="cb530-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb530-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

### <a name="response"></a><span data-ttu-id="cb530-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb530-133">Response</span></span>
<span data-ttu-id="cb530-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb530-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 869

{
  "value": [
    {
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
  ]
}
```





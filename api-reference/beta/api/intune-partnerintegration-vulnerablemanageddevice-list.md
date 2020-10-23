---
title: Listar vulnerableManagedDevices
description: Listar Propriedades e relações dos objetos vulnerableManagedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2f45ada8bfccad2c9e3c46e5ef370a78e4efa2a6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692902"
---
# <a name="list-vulnerablemanageddevices"></a><span data-ttu-id="f2f3d-103">Listar vulnerableManagedDevices</span><span class="sxs-lookup"><span data-stu-id="f2f3d-103">List vulnerableManagedDevices</span></span>

<span data-ttu-id="f2f3d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2f3d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2f3d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2f3d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2f3d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2f3d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2f3d-107">Listar Propriedades e relações dos objetos [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="f2f3d-107">List properties and relationships of the [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2f3d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2f3d-108">Prerequisites</span></span>
<span data-ttu-id="f2f3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2f3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2f3d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2f3d-111">Permission type</span></span>|<span data-ttu-id="f2f3d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2f3d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2f3d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2f3d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2f3d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2f3d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f2f3d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2f3d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2f3d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2f3d-116">Not supported.</span></span>|
|<span data-ttu-id="f2f3d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2f3d-117">Application</span></span>|<span data-ttu-id="f2f3d-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2f3d-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2f3d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2f3d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET ** Collection URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

## <a name="request-headers"></a><span data-ttu-id="f2f3d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2f3d-120">Request headers</span></span>
|<span data-ttu-id="f2f3d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2f3d-121">Header</span></span>|<span data-ttu-id="f2f3d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f2f3d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2f3d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2f3d-123">Authorization</span></span>|<span data-ttu-id="f2f3d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2f3d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2f3d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2f3d-125">Accept</span></span>|<span data-ttu-id="f2f3d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2f3d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2f3d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2f3d-127">Request body</span></span>
<span data-ttu-id="f2f3d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2f3d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2f3d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2f3d-129">Response</span></span>
<span data-ttu-id="f2f3d-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2f3d-130">If successful, this method returns a `200 OK` response code and a collection of [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2f3d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2f3d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2f3d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2f3d-132">Request</span></span>
<span data-ttu-id="f2f3d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2f3d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

### <a name="response"></a><span data-ttu-id="f2f3d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2f3d-134">Response</span></span>
<span data-ttu-id="f2f3d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2f3d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 316

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
      "id": "e59891d4-91d4-e598-d491-98e5d49198e5",
      "managedDeviceId": "Managed Device Id value",
      "displayName": "Display Name value",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
    }
  ]
}
```






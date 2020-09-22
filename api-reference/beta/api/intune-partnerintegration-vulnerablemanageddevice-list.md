---
title: Listar vulnerableManagedDevices
description: Listar Propriedades e relações dos objetos vulnerableManagedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c3f11a0c78a0a4c30b916540af3defa7f5f327e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999927"
---
# <a name="list-vulnerablemanageddevices"></a><span data-ttu-id="c0923-103">Listar vulnerableManagedDevices</span><span class="sxs-lookup"><span data-stu-id="c0923-103">List vulnerableManagedDevices</span></span>

<span data-ttu-id="c0923-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0923-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0923-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0923-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0923-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0923-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0923-107">Listar Propriedades e relações dos objetos [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="c0923-107">List properties and relationships of the [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0923-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0923-108">Prerequisites</span></span>
<span data-ttu-id="c0923-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0923-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0923-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0923-111">Permission type</span></span>|<span data-ttu-id="c0923-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c0923-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0923-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0923-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0923-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0923-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c0923-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0923-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0923-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0923-116">Not supported.</span></span>|
|<span data-ttu-id="c0923-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0923-117">Application</span></span>|<span data-ttu-id="c0923-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0923-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0923-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0923-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET ** Collection URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

## <a name="request-headers"></a><span data-ttu-id="c0923-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0923-120">Request headers</span></span>
|<span data-ttu-id="c0923-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0923-121">Header</span></span>|<span data-ttu-id="c0923-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c0923-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0923-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0923-123">Authorization</span></span>|<span data-ttu-id="c0923-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0923-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0923-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c0923-125">Accept</span></span>|<span data-ttu-id="c0923-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0923-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0923-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0923-127">Request body</span></span>
<span data-ttu-id="c0923-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0923-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0923-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0923-129">Response</span></span>
<span data-ttu-id="c0923-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0923-130">If successful, this method returns a `200 OK` response code and a collection of [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0923-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0923-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0923-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0923-132">Request</span></span>
<span data-ttu-id="c0923-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0923-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

### <a name="response"></a><span data-ttu-id="c0923-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0923-134">Response</span></span>
<span data-ttu-id="c0923-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0923-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







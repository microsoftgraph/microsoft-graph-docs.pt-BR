---
title: Listar vulnerableManagedDevices
description: Listar propriedades e relações dos objetos vulnerableManagedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 95a1c0f811a59aac2b9de7445e361fa3f2feb01b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145254"
---
# <a name="list-vulnerablemanageddevices"></a><span data-ttu-id="c8496-103">Listar vulnerableManagedDevices</span><span class="sxs-lookup"><span data-stu-id="c8496-103">List vulnerableManagedDevices</span></span>

<span data-ttu-id="c8496-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8496-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8496-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8496-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8496-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8496-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8496-107">Listar propriedades e relações dos [objetos vulnerableManagedDevice.](../resources/intune-partnerintegration-vulnerablemanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c8496-107">List properties and relationships of the [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8496-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c8496-108">Prerequisites</span></span>
<span data-ttu-id="c8496-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8496-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8496-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8496-111">Permission type</span></span>|<span data-ttu-id="c8496-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c8496-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8496-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8496-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8496-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8496-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c8496-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8496-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8496-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8496-116">Not supported.</span></span>|
|<span data-ttu-id="c8496-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8496-117">Application</span></span>|<span data-ttu-id="c8496-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8496-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8496-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8496-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET ** Collection URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

## <a name="request-headers"></a><span data-ttu-id="c8496-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8496-120">Request headers</span></span>
|<span data-ttu-id="c8496-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8496-121">Header</span></span>|<span data-ttu-id="c8496-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c8496-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8496-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8496-123">Authorization</span></span>|<span data-ttu-id="c8496-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8496-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8496-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c8496-125">Accept</span></span>|<span data-ttu-id="c8496-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8496-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8496-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8496-127">Request body</span></span>
<span data-ttu-id="c8496-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8496-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8496-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8496-129">Response</span></span>
<span data-ttu-id="c8496-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8496-130">If successful, this method returns a `200 OK` response code and a collection of [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8496-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8496-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8496-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8496-132">Request</span></span>
<span data-ttu-id="c8496-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8496-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

### <a name="response"></a><span data-ttu-id="c8496-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8496-134">Response</span></span>
<span data-ttu-id="c8496-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8496-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





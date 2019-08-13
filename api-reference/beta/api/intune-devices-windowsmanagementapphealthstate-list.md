---
title: Listar windowsManagementAppHealthStates
description: Listar Propriedades e relações dos objetos windowsManagementAppHealthState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d46ff77e3e8d08c1e392e507a695c3bbd7e51da6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309846"
---
# <a name="list-windowsmanagementapphealthstates"></a><span data-ttu-id="c8f0a-103">Listar windowsManagementAppHealthStates</span><span class="sxs-lookup"><span data-stu-id="c8f0a-103">List windowsManagementAppHealthStates</span></span>

> <span data-ttu-id="c8f0a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8f0a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8f0a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8f0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8f0a-106">Listar Propriedades e relações dos objetos [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="c8f0a-106">List properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8f0a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c8f0a-107">Prerequisites</span></span>
<span data-ttu-id="c8f0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8f0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8f0a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8f0a-110">Permission type</span></span>|<span data-ttu-id="c8f0a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c8f0a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8f0a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8f0a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8f0a-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8f0a-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c8f0a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8f0a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8f0a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8f0a-115">Not supported.</span></span>|
|<span data-ttu-id="c8f0a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8f0a-116">Application</span></span>|<span data-ttu-id="c8f0a-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8f0a-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8f0a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8f0a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="c8f0a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8f0a-119">Request headers</span></span>
|<span data-ttu-id="c8f0a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8f0a-120">Header</span></span>|<span data-ttu-id="c8f0a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c8f0a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8f0a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8f0a-122">Authorization</span></span>|<span data-ttu-id="c8f0a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8f0a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8f0a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c8f0a-124">Accept</span></span>|<span data-ttu-id="c8f0a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c8f0a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8f0a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8f0a-126">Request body</span></span>
<span data-ttu-id="c8f0a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8f0a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8f0a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8f0a-128">Response</span></span>
<span data-ttu-id="c8f0a-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8f0a-129">If successful, this method returns a `200 OK` response code and a collection of [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8f0a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8f0a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8f0a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8f0a-131">Request</span></span>
<span data-ttu-id="c8f0a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8f0a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates
```

### <a name="response"></a><span data-ttu-id="c8f0a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8f0a-133">Response</span></span>
<span data-ttu-id="c8f0a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8f0a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 410

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
      "id": "5c7e50fb-50fb-5c7e-fb50-7e5cfb507e5c",
      "healthState": "healthy",
      "installedVersion": "Installed Version value",
      "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
      "deviceName": "Device Name value",
      "deviceOSVersion": "Device OSVersion value"
    }
  ]
}
```







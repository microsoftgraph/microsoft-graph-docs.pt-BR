---
title: Listar windowsManagementAppHealthStates
description: Listar Propriedades e relações dos objetos windowsManagementAppHealthState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1b48f9edc91fa190f2963885454f1897423ff863
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49228369"
---
# <a name="list-windowsmanagementapphealthstates"></a><span data-ttu-id="adf51-103">Listar windowsManagementAppHealthStates</span><span class="sxs-lookup"><span data-stu-id="adf51-103">List windowsManagementAppHealthStates</span></span>

<span data-ttu-id="adf51-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adf51-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="adf51-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="adf51-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adf51-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="adf51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adf51-107">Listar Propriedades e relações dos objetos [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="adf51-107">List properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="adf51-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="adf51-108">Prerequisites</span></span>
<span data-ttu-id="adf51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adf51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adf51-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="adf51-111">Permission type</span></span>|<span data-ttu-id="adf51-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="adf51-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adf51-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="adf51-113">Delegated (work or school account)</span></span>|<span data-ttu-id="adf51-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="adf51-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="adf51-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="adf51-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adf51-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adf51-116">Not supported.</span></span>|
|<span data-ttu-id="adf51-117">Application</span><span class="sxs-lookup"><span data-stu-id="adf51-117">Application</span></span>|<span data-ttu-id="adf51-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="adf51-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="adf51-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adf51-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="adf51-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="adf51-120">Request headers</span></span>
|<span data-ttu-id="adf51-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="adf51-121">Header</span></span>|<span data-ttu-id="adf51-122">Valor</span><span class="sxs-lookup"><span data-stu-id="adf51-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adf51-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="adf51-123">Authorization</span></span>|<span data-ttu-id="adf51-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="adf51-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adf51-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="adf51-125">Accept</span></span>|<span data-ttu-id="adf51-126">application/json</span><span class="sxs-lookup"><span data-stu-id="adf51-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adf51-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="adf51-127">Request body</span></span>
<span data-ttu-id="adf51-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="adf51-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adf51-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="adf51-129">Response</span></span>
<span data-ttu-id="adf51-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="adf51-130">If successful, this method returns a `200 OK` response code and a collection of [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adf51-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="adf51-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="adf51-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="adf51-132">Request</span></span>
<span data-ttu-id="adf51-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="adf51-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates
```

### <a name="response"></a><span data-ttu-id="adf51-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="adf51-134">Response</span></span>
<span data-ttu-id="adf51-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="adf51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





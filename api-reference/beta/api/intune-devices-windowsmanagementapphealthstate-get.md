---
title: Obter windowsManagementAppHealthState
description: Leia as propriedades e as relações do objeto windowsManagementAppHealthState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: faa6909676e95bd304bd38a9b2490fbd78393481
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188028"
---
# <a name="get-windowsmanagementapphealthstate"></a><span data-ttu-id="fdaaf-103">Obter windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="fdaaf-103">Get windowsManagementAppHealthState</span></span>

> <span data-ttu-id="fdaaf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fdaaf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdaaf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fdaaf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdaaf-106">Leia as propriedades e as relações do objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="fdaaf-106">Read properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdaaf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fdaaf-107">Prerequisites</span></span>
<span data-ttu-id="fdaaf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdaaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdaaf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdaaf-110">Permission type</span></span>|<span data-ttu-id="fdaaf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fdaaf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdaaf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdaaf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fdaaf-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdaaf-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="fdaaf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdaaf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdaaf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdaaf-115">Not supported.</span></span>|
|<span data-ttu-id="fdaaf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdaaf-116">Application</span></span>|<span data-ttu-id="fdaaf-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdaaf-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdaaf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdaaf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fdaaf-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fdaaf-119">Optional query parameters</span></span>
<span data-ttu-id="fdaaf-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fdaaf-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fdaaf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdaaf-121">Request headers</span></span>
|<span data-ttu-id="fdaaf-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fdaaf-122">Header</span></span>|<span data-ttu-id="fdaaf-123">Valor</span><span class="sxs-lookup"><span data-stu-id="fdaaf-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdaaf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdaaf-124">Authorization</span></span>|<span data-ttu-id="fdaaf-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdaaf-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdaaf-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fdaaf-126">Accept</span></span>|<span data-ttu-id="fdaaf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fdaaf-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdaaf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdaaf-128">Request body</span></span>
<span data-ttu-id="fdaaf-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fdaaf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdaaf-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdaaf-130">Response</span></span>
<span data-ttu-id="fdaaf-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdaaf-131">If successful, this method returns a `200 OK` response code and [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdaaf-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdaaf-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdaaf-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdaaf-133">Request</span></span>
<span data-ttu-id="fdaaf-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdaaf-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

### <a name="response"></a><span data-ttu-id="fdaaf-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdaaf-135">Response</span></span>
<span data-ttu-id="fdaaf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdaaf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 382

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
    "id": "5c7e50fb-50fb-5c7e-fb50-7e5cfb507e5c",
    "healthState": "healthy",
    "installedVersion": "Installed Version value",
    "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
    "deviceName": "Device Name value",
    "deviceOSVersion": "Device OSVersion value"
  }
}
```





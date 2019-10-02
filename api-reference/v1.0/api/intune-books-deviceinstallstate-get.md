---
title: Get deviceInstallState
description: Ler propriedades e relações do objeto deviceInstallState.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 22c1e5a7f00000f10aa832143eeca8f0b430c571
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354830"
---
# <a name="get-deviceinstallstate"></a><span data-ttu-id="e1487-103">Get deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="e1487-103">Get deviceInstallState</span></span>

> <span data-ttu-id="e1487-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1487-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1487-105">Ler propriedades e relações do objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="e1487-105">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1487-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1487-106">Prerequisites</span></span>
<span data-ttu-id="e1487-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1487-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1487-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1487-109">Permission type</span></span>|<span data-ttu-id="e1487-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1487-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1487-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1487-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e1487-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1487-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e1487-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1487-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1487-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1487-114">Not supported.</span></span>|
|<span data-ttu-id="e1487-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1487-115">Application</span></span>|<span data-ttu-id="e1487-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1487-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1487-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1487-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1487-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e1487-118">Optional query parameters</span></span>
<span data-ttu-id="e1487-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e1487-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1487-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1487-120">Request headers</span></span>
|<span data-ttu-id="e1487-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1487-121">Header</span></span>|<span data-ttu-id="e1487-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e1487-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1487-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1487-123">Authorization</span></span>|<span data-ttu-id="e1487-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1487-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1487-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1487-125">Accept</span></span>|<span data-ttu-id="e1487-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1487-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1487-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1487-127">Request body</span></span>
<span data-ttu-id="e1487-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1487-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1487-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1487-129">Response</span></span>
<span data-ttu-id="e1487-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1487-130">If successful, this method returns a `200 OK` response code and [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1487-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1487-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1487-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1487-132">Request</span></span>
<span data-ttu-id="e1487-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1487-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="e1487-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1487-134">Response</span></span>
<span data-ttu-id="e1487-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1487-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 462

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceInstallState",
    "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
    "deviceName": "Device Name value",
    "deviceId": "Device Id value",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "installState": "installed",
    "errorCode": "Error Code value",
    "osVersion": "Os Version value",
    "osDescription": "Os Description value",
    "userName": "User Name value"
  }
}
```





---
title: Get deviceInstallState
description: Ler propriedades e relações do objeto deviceInstallState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c47b1827ae55da6456603b810287c431ed7fcc54
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48716919"
---
# <a name="get-deviceinstallstate"></a><span data-ttu-id="f582b-103">Get deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="f582b-103">Get deviceInstallState</span></span>

<span data-ttu-id="f582b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f582b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f582b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f582b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f582b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f582b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f582b-107">Ler propriedades e relações do objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="f582b-107">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f582b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f582b-108">Prerequisites</span></span>
<span data-ttu-id="f582b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f582b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f582b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f582b-111">Permission type</span></span>|<span data-ttu-id="f582b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f582b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f582b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f582b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f582b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f582b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f582b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f582b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f582b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f582b-116">Not supported.</span></span>|
|<span data-ttu-id="f582b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f582b-117">Application</span></span>|<span data-ttu-id="f582b-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f582b-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f582b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f582b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f582b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f582b-120">Optional query parameters</span></span>
<span data-ttu-id="f582b-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f582b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f582b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f582b-122">Request headers</span></span>
|<span data-ttu-id="f582b-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f582b-123">Header</span></span>|<span data-ttu-id="f582b-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f582b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f582b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f582b-125">Authorization</span></span>|<span data-ttu-id="f582b-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f582b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f582b-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f582b-127">Accept</span></span>|<span data-ttu-id="f582b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f582b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f582b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f582b-129">Request body</span></span>
<span data-ttu-id="f582b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f582b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f582b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f582b-131">Response</span></span>
<span data-ttu-id="f582b-132">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f582b-132">If successful, this method returns a `200 OK` response code and [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f582b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f582b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f582b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f582b-134">Request</span></span>
<span data-ttu-id="f582b-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f582b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="f582b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f582b-136">Response</span></span>
<span data-ttu-id="f582b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f582b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






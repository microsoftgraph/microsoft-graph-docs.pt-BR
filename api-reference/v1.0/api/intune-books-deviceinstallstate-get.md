---
title: Get deviceInstallState
description: Ler propriedades e relações do objeto deviceInstallState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e9ca55b2805a925f7fed2dab263951bd9907ad26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980430"
---
# <a name="get-deviceinstallstate"></a><span data-ttu-id="2b2a1-103">Get deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="2b2a1-103">Get deviceInstallState</span></span>

> <span data-ttu-id="2b2a1-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2b2a1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b2a1-105">Ler propriedades e relações do objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="2b2a1-105">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b2a1-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2b2a1-106">Prerequisites</span></span>
<span data-ttu-id="2b2a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b2a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b2a1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b2a1-109">Permission type</span></span>|<span data-ttu-id="2b2a1-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2b2a1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b2a1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b2a1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2b2a1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b2a1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2b2a1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b2a1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b2a1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b2a1-114">Not supported.</span></span>|
|<span data-ttu-id="2b2a1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b2a1-115">Application</span></span>|<span data-ttu-id="2b2a1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b2a1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b2a1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b2a1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b2a1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2b2a1-118">Optional query parameters</span></span>
<span data-ttu-id="2b2a1-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2b2a1-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2b2a1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b2a1-120">Request headers</span></span>
|<span data-ttu-id="2b2a1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2b2a1-121">Header</span></span>|<span data-ttu-id="2b2a1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2b2a1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b2a1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b2a1-123">Authorization</span></span>|<span data-ttu-id="2b2a1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b2a1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b2a1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2b2a1-125">Accept</span></span>|<span data-ttu-id="2b2a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b2a1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b2a1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b2a1-127">Request body</span></span>
<span data-ttu-id="2b2a1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b2a1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b2a1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b2a1-129">Response</span></span>
<span data-ttu-id="2b2a1-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b2a1-130">If successful, this method returns a `200 OK` response code and [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b2a1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b2a1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b2a1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b2a1-132">Request</span></span>
<span data-ttu-id="2b2a1-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b2a1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="2b2a1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b2a1-134">Response</span></span>
<span data-ttu-id="2b2a1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b2a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




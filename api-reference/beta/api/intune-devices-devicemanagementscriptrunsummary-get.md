---
title: Obter deviceManagementScriptRunSummary
description: Leia as propriedades e as relações do objeto deviceManagementScriptRunSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d66d68de179b3b6a36312d6b25d4ff81f9fc6d5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144965"
---
# <a name="get-devicemanagementscriptrunsummary"></a><span data-ttu-id="e4776-103">Obter deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="e4776-103">Get deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="e4776-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4776-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4776-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4776-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4776-106">Leia as propriedades e as relações do objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="e4776-106">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4776-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4776-107">Prerequisites</span></span>
<span data-ttu-id="e4776-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e4776-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e4776-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4776-110">Permission type</span></span>|<span data-ttu-id="e4776-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4776-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4776-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4776-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4776-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4776-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e4776-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4776-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4776-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4776-115">Not supported.</span></span>|
|<span data-ttu-id="e4776-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4776-116">Application</span></span>|<span data-ttu-id="e4776-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4776-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4776-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4776-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4776-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e4776-119">Optional query parameters</span></span>
<span data-ttu-id="e4776-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e4776-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4776-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4776-121">Request headers</span></span>
|<span data-ttu-id="e4776-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4776-122">Header</span></span>|<span data-ttu-id="e4776-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e4776-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4776-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4776-124">Authorization</span></span>|<span data-ttu-id="e4776-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4776-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4776-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e4776-126">Accept</span></span>|<span data-ttu-id="e4776-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e4776-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4776-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4776-128">Request body</span></span>
<span data-ttu-id="e4776-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4776-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4776-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4776-130">Response</span></span>
<span data-ttu-id="e4776-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4776-131">If successful, this method returns a `200 OK` response code and [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4776-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4776-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4776-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4776-133">Request</span></span>
<span data-ttu-id="e4776-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4776-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

### <a name="response"></a><span data-ttu-id="e4776-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4776-135">Response</span></span>
<span data-ttu-id="e4776-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4776-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
    "id": "514d5d38-5d38-514d-385d-4d51385d4d51",
    "successDeviceCount": 2,
    "errorDeviceCount": 0,
    "successUserCount": 0,
    "errorUserCount": 14
  }
}
```





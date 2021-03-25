---
title: Obter deviceManagementScriptRunSummary
description: Ler propriedades e relações do objeto deviceManagementScriptRunSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f633e067c6d605ee6c0b44e7833bfa369976d400
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150392"
---
# <a name="get-devicemanagementscriptrunsummary"></a><span data-ttu-id="28c63-103">Obter deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="28c63-103">Get deviceManagementScriptRunSummary</span></span>

<span data-ttu-id="28c63-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28c63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28c63-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="28c63-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28c63-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28c63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28c63-107">Ler propriedades e relações do [objeto deviceManagementScriptRunSummary.](../resources/intune-devices-devicemanagementscriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="28c63-107">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28c63-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="28c63-108">Prerequisites</span></span>
<span data-ttu-id="28c63-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28c63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28c63-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28c63-111">Permission type</span></span>|<span data-ttu-id="28c63-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28c63-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28c63-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28c63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28c63-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28c63-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="28c63-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28c63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28c63-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28c63-116">Not supported.</span></span>|
|<span data-ttu-id="28c63-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28c63-117">Application</span></span>|<span data-ttu-id="28c63-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28c63-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28c63-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28c63-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
GET /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/runSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28c63-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="28c63-120">Optional query parameters</span></span>
<span data-ttu-id="28c63-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="28c63-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28c63-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28c63-122">Request headers</span></span>
|<span data-ttu-id="28c63-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28c63-123">Header</span></span>|<span data-ttu-id="28c63-124">Valor</span><span class="sxs-lookup"><span data-stu-id="28c63-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28c63-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="28c63-125">Authorization</span></span>|<span data-ttu-id="28c63-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28c63-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28c63-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="28c63-127">Accept</span></span>|<span data-ttu-id="28c63-128">application/json</span><span class="sxs-lookup"><span data-stu-id="28c63-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28c63-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28c63-129">Request body</span></span>
<span data-ttu-id="28c63-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28c63-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28c63-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="28c63-131">Response</span></span>
<span data-ttu-id="28c63-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28c63-132">If successful, this method returns a `200 OK` response code and [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28c63-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28c63-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="28c63-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28c63-134">Request</span></span>
<span data-ttu-id="28c63-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28c63-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
```

### <a name="response"></a><span data-ttu-id="28c63-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="28c63-136">Response</span></span>
<span data-ttu-id="28c63-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28c63-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





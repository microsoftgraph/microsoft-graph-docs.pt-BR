---
title: Get detectedApp
description: Ler propriedades e relações do objeto detectedApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b182ebe67d481d3f800b9b1e1e76749b9f1055d9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769616"
---
# <a name="get-detectedapp"></a><span data-ttu-id="948f8-103">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="948f8-103">Get detectedApp</span></span>

> <span data-ttu-id="948f8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="948f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="948f8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="948f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="948f8-106">Ler propriedades e relações do objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="948f8-106">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="948f8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="948f8-107">Prerequisites</span></span>
<span data-ttu-id="948f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="948f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="948f8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="948f8-110">Permission type</span></span>|<span data-ttu-id="948f8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="948f8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="948f8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="948f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="948f8-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="948f8-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="948f8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="948f8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="948f8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="948f8-115">Not supported.</span></span>|
|<span data-ttu-id="948f8-116">Application</span><span class="sxs-lookup"><span data-stu-id="948f8-116">Application</span></span>|<span data-ttu-id="948f8-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="948f8-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="948f8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="948f8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="948f8-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="948f8-119">Optional query parameters</span></span>
<span data-ttu-id="948f8-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="948f8-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="948f8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="948f8-121">Request headers</span></span>
|<span data-ttu-id="948f8-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="948f8-122">Header</span></span>|<span data-ttu-id="948f8-123">Valor</span><span class="sxs-lookup"><span data-stu-id="948f8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="948f8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="948f8-124">Authorization</span></span>|<span data-ttu-id="948f8-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="948f8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="948f8-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="948f8-126">Accept</span></span>|<span data-ttu-id="948f8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="948f8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="948f8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="948f8-128">Request body</span></span>
<span data-ttu-id="948f8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="948f8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="948f8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="948f8-130">Response</span></span>
<span data-ttu-id="948f8-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [detectedApp](../resources/intune-devices-detectedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="948f8-131">If successful, this method returns a `200 OK` response code and [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="948f8-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="948f8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="948f8-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="948f8-133">Request</span></span>
<span data-ttu-id="948f8-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="948f8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
```

### <a name="response"></a><span data-ttu-id="948f8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="948f8-135">Response</span></span>
<span data-ttu-id="948f8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="948f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "value": {
    "@odata.type": "#microsoft.graph.detectedApp",
    "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
    "displayName": "Display Name value",
    "version": "Version value",
    "sizeInByte": 10,
    "deviceCount": 11
  }
}
```





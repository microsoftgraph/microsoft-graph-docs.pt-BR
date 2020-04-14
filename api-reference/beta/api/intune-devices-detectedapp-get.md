---
title: Get detectedApp
description: Ler propriedades e relações do objeto detectedApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a7f8bc26217230dc5d79fd137c86fc210d366a90
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43426516"
---
# <a name="get-detectedapp"></a><span data-ttu-id="fc754-103">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="fc754-103">Get detectedApp</span></span>

<span data-ttu-id="fc754-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc754-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc754-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fc754-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc754-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc754-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc754-107">Ler propriedades e relações do objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="fc754-107">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc754-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fc754-108">Prerequisites</span></span>
<span data-ttu-id="fc754-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc754-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc754-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc754-111">Permission type</span></span>|<span data-ttu-id="fc754-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fc754-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc754-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc754-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc754-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc754-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="fc754-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc754-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc754-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc754-116">Not supported.</span></span>|
|<span data-ttu-id="fc754-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc754-117">Application</span></span>|<span data-ttu-id="fc754-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc754-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc754-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc754-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc754-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fc754-120">Optional query parameters</span></span>
<span data-ttu-id="fc754-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fc754-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc754-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc754-122">Request headers</span></span>
|<span data-ttu-id="fc754-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc754-123">Header</span></span>|<span data-ttu-id="fc754-124">Valor</span><span class="sxs-lookup"><span data-stu-id="fc754-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc754-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc754-125">Authorization</span></span>|<span data-ttu-id="fc754-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc754-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc754-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fc754-127">Accept</span></span>|<span data-ttu-id="fc754-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fc754-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc754-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc754-129">Request body</span></span>
<span data-ttu-id="fc754-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc754-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc754-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc754-131">Response</span></span>
<span data-ttu-id="fc754-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [detectedApp](../resources/intune-devices-detectedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc754-132">If successful, this method returns a `200 OK` response code and [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc754-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc754-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc754-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc754-134">Request</span></span>
<span data-ttu-id="fc754-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc754-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
```

### <a name="response"></a><span data-ttu-id="fc754-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc754-136">Response</span></span>
<span data-ttu-id="fc754-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc754-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




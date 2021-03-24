---
title: Get detectedApp
description: Ler propriedades e relações do objeto detectedApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 59d1cad746c75a4ce6a970ed96fc1cdd63f6a8c4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146500"
---
# <a name="get-detectedapp"></a><span data-ttu-id="b1aeb-103">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="b1aeb-103">Get detectedApp</span></span>

<span data-ttu-id="b1aeb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1aeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1aeb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1aeb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1aeb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1aeb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1aeb-107">Ler propriedades e relações do objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1aeb-107">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1aeb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b1aeb-108">Prerequisites</span></span>
<span data-ttu-id="b1aeb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1aeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1aeb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1aeb-111">Permission type</span></span>|<span data-ttu-id="b1aeb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1aeb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1aeb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1aeb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1aeb-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1aeb-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b1aeb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1aeb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1aeb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1aeb-116">Not supported.</span></span>|
|<span data-ttu-id="b1aeb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1aeb-117">Application</span></span>|<span data-ttu-id="b1aeb-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1aeb-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1aeb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1aeb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b1aeb-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b1aeb-120">Optional query parameters</span></span>
<span data-ttu-id="b1aeb-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b1aeb-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1aeb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1aeb-122">Request headers</span></span>
|<span data-ttu-id="b1aeb-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1aeb-123">Header</span></span>|<span data-ttu-id="b1aeb-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b1aeb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1aeb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1aeb-125">Authorization</span></span>|<span data-ttu-id="b1aeb-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1aeb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1aeb-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b1aeb-127">Accept</span></span>|<span data-ttu-id="b1aeb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b1aeb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1aeb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1aeb-129">Request body</span></span>
<span data-ttu-id="b1aeb-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b1aeb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1aeb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1aeb-131">Response</span></span>
<span data-ttu-id="b1aeb-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [detectedApp](../resources/intune-devices-detectedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1aeb-132">If successful, this method returns a `200 OK` response code and [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1aeb-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1aeb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1aeb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1aeb-134">Request</span></span>
<span data-ttu-id="b1aeb-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1aeb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
```

### <a name="response"></a><span data-ttu-id="b1aeb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1aeb-136">Response</span></span>
<span data-ttu-id="b1aeb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1aeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





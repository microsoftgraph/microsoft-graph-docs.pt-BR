---
title: Listar detectedApps
description: Listar propriedades e relações dos objetos detectedApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 90a32db07db00f0d1eec4f2c1320c6351a417e78
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146465"
---
# <a name="list-detectedapps"></a><span data-ttu-id="b7a21-103">Listar detectedApps</span><span class="sxs-lookup"><span data-stu-id="b7a21-103">List detectedApps</span></span>

<span data-ttu-id="b7a21-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7a21-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7a21-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b7a21-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7a21-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7a21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7a21-107">Listar propriedades e relações dos objetos [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7a21-107">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7a21-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7a21-108">Prerequisites</span></span>
<span data-ttu-id="b7a21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7a21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7a21-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7a21-111">Permission type</span></span>|<span data-ttu-id="b7a21-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7a21-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7a21-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7a21-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7a21-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7a21-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b7a21-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7a21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7a21-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7a21-116">Not supported.</span></span>|
|<span data-ttu-id="b7a21-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7a21-117">Application</span></span>|<span data-ttu-id="b7a21-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7a21-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7a21-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7a21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="b7a21-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7a21-120">Request headers</span></span>
|<span data-ttu-id="b7a21-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7a21-121">Header</span></span>|<span data-ttu-id="b7a21-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b7a21-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7a21-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7a21-123">Authorization</span></span>|<span data-ttu-id="b7a21-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7a21-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7a21-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b7a21-125">Accept</span></span>|<span data-ttu-id="b7a21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7a21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7a21-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7a21-127">Request body</span></span>
<span data-ttu-id="b7a21-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b7a21-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7a21-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7a21-129">Response</span></span>
<span data-ttu-id="b7a21-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [detectedApp](../resources/intune-devices-detectedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7a21-130">If successful, this method returns a `200 OK` response code and a collection of [detectedApp](../resources/intune-devices-detectedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7a21-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7a21-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7a21-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7a21-132">Request</span></span>
<span data-ttu-id="b7a21-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7a21-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/detectedApps
```

### <a name="response"></a><span data-ttu-id="b7a21-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7a21-134">Response</span></span>
<span data-ttu-id="b7a21-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7a21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.detectedApp",
      "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
      "displayName": "Display Name value",
      "version": "Version value",
      "sizeInByte": 10,
      "deviceCount": 11
    }
  ]
}
```





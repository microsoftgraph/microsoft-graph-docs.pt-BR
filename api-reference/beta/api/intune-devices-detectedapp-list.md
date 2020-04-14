---
title: Listar detectedApps
description: Listar propriedades e relações dos objetos detectedApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b8540d4ec02071a01cebd799d73250dcf5426bf7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43380999"
---
# <a name="list-detectedapps"></a><span data-ttu-id="5a56f-103">Listar detectedApps</span><span class="sxs-lookup"><span data-stu-id="5a56f-103">List detectedApps</span></span>

<span data-ttu-id="5a56f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a56f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a56f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5a56f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a56f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5a56f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a56f-107">Listar propriedades e relações dos objetos [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a56f-107">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a56f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5a56f-108">Prerequisites</span></span>
<span data-ttu-id="5a56f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a56f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a56f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a56f-111">Permission type</span></span>|<span data-ttu-id="5a56f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5a56f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a56f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a56f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5a56f-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a56f-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5a56f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a56f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a56f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a56f-116">Not supported.</span></span>|
|<span data-ttu-id="5a56f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a56f-117">Application</span></span>|<span data-ttu-id="5a56f-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a56f-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a56f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a56f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="5a56f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a56f-120">Request headers</span></span>
|<span data-ttu-id="5a56f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5a56f-121">Header</span></span>|<span data-ttu-id="5a56f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5a56f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a56f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a56f-123">Authorization</span></span>|<span data-ttu-id="5a56f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a56f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a56f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5a56f-125">Accept</span></span>|<span data-ttu-id="5a56f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5a56f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a56f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a56f-127">Request body</span></span>
<span data-ttu-id="5a56f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a56f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a56f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a56f-129">Response</span></span>
<span data-ttu-id="5a56f-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [detectedApp](../resources/intune-devices-detectedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a56f-130">If successful, this method returns a `200 OK` response code and a collection of [detectedApp](../resources/intune-devices-detectedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a56f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a56f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a56f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a56f-132">Request</span></span>
<span data-ttu-id="5a56f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a56f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/detectedApps
```

### <a name="response"></a><span data-ttu-id="5a56f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a56f-134">Response</span></span>
<span data-ttu-id="5a56f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a56f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




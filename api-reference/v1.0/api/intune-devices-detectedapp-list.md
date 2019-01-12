---
title: Listar detectedApps
description: Listar propriedades e relações dos objetos detectedApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 53c84c652f41a251de70ff3bd872e1789f0a184a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932347"
---
# <a name="list-detectedapps"></a><span data-ttu-id="003e6-103">Listar detectedApps</span><span class="sxs-lookup"><span data-stu-id="003e6-103">List detectedApps</span></span>

> <span data-ttu-id="003e6-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="003e6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="003e6-105">Listar propriedades e relações dos objetos [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="003e6-105">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="003e6-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="003e6-106">Prerequisites</span></span>
<span data-ttu-id="003e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="003e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="003e6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="003e6-109">Permission type</span></span>|<span data-ttu-id="003e6-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="003e6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="003e6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="003e6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="003e6-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="003e6-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="003e6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="003e6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="003e6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="003e6-114">Not supported.</span></span>|
|<span data-ttu-id="003e6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="003e6-115">Application</span></span>|<span data-ttu-id="003e6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="003e6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="003e6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="003e6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="003e6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="003e6-118">Request headers</span></span>
|<span data-ttu-id="003e6-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="003e6-119">Header</span></span>|<span data-ttu-id="003e6-120">Valor</span><span class="sxs-lookup"><span data-stu-id="003e6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="003e6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="003e6-121">Authorization</span></span>|<span data-ttu-id="003e6-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="003e6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="003e6-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="003e6-123">Accept</span></span>|<span data-ttu-id="003e6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="003e6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="003e6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="003e6-125">Request body</span></span>
<span data-ttu-id="003e6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="003e6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="003e6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="003e6-127">Response</span></span>
<span data-ttu-id="003e6-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [detectedApp](../resources/intune-devices-detectedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="003e6-128">If successful, this method returns a `200 OK` response code and a collection of [detectedApp](../resources/intune-devices-detectedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="003e6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="003e6-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="003e6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="003e6-130">Request</span></span>
<span data-ttu-id="003e6-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="003e6-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
```

### <a name="response"></a><span data-ttu-id="003e6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="003e6-132">Response</span></span>
<span data-ttu-id="003e6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="003e6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




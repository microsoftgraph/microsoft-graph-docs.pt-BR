---
title: Listar iosManagedAppRegistrations
description: Lista propriedades e relações dos objetos iosManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a822a4c26dc8f78bad3fde90898390817a84bcac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974347"
---
# <a name="list-iosmanagedappregistrations"></a><span data-ttu-id="41d3a-103">Listar iosManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="41d3a-103">List iosManagedAppRegistrations</span></span>

> <span data-ttu-id="41d3a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="41d3a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41d3a-105">Listar propriedades e relações dos objetos [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="41d3a-105">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41d3a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41d3a-106">Prerequisites</span></span>
<span data-ttu-id="41d3a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41d3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41d3a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41d3a-109">Permission type</span></span>|<span data-ttu-id="41d3a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="41d3a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41d3a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41d3a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="41d3a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="41d3a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="41d3a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41d3a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41d3a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41d3a-114">Not supported.</span></span>|
|<span data-ttu-id="41d3a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41d3a-115">Application</span></span>|<span data-ttu-id="41d3a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41d3a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41d3a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41d3a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="41d3a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41d3a-118">Request headers</span></span>
|<span data-ttu-id="41d3a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41d3a-119">Header</span></span>|<span data-ttu-id="41d3a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="41d3a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41d3a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="41d3a-121">Authorization</span></span>|<span data-ttu-id="41d3a-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41d3a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41d3a-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41d3a-123">Accept</span></span>|<span data-ttu-id="41d3a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="41d3a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41d3a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41d3a-125">Request body</span></span>
<span data-ttu-id="41d3a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41d3a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41d3a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="41d3a-127">Response</span></span>
<span data-ttu-id="41d3a-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41d3a-128">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41d3a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41d3a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="41d3a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41d3a-130">Request</span></span>
<span data-ttu-id="41d3a-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41d3a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="41d3a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="41d3a-132">Response</span></span>
<span data-ttu-id="41d3a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41d3a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 852

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "applicationVersion": "Application Version value",
      "managementSdkVersion": "Management Sdk Version value",
      "platformVersion": "Platform Version value",
      "deviceType": "Device Type value",
      "deviceTag": "Device Tag value",
      "deviceName": "Device Name value",
      "flaggedReasons": [
        "rootedDevice"
      ],
      "userId": "User Id value",
      "appIdentifier": {
        "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
        "bundleId": "Bundle Id value"
      },
      "id": "47632c19-2c19-4763-192c-6347192c6347",
      "version": "Version value"
    }
  ]
}
```




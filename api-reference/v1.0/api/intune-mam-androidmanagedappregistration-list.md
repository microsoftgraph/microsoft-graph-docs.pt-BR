---
title: Listar androidManagedAppRegistrations
description: Lista propriedades e relações dos objetos androidManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 14169256c0aae4eea6d8190575c9519213dc3293
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254923"
---
# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="a1af3-103">Listar androidManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="a1af3-103">List androidManagedAppRegistrations</span></span>

> <span data-ttu-id="a1af3-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1af3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1af3-105">Listar propriedades e relações dos objetos [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a1af3-105">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1af3-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1af3-106">Prerequisites</span></span>
<span data-ttu-id="a1af3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a1af3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a1af3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1af3-109">Permission type</span></span>|<span data-ttu-id="a1af3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1af3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1af3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1af3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a1af3-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1af3-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a1af3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1af3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1af3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1af3-114">Not supported.</span></span>|
|<span data-ttu-id="a1af3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1af3-115">Application</span></span>|<span data-ttu-id="a1af3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1af3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1af3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1af3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="a1af3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1af3-118">Request headers</span></span>
|<span data-ttu-id="a1af3-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1af3-119">Header</span></span>|<span data-ttu-id="a1af3-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a1af3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1af3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1af3-121">Authorization</span></span>|<span data-ttu-id="a1af3-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1af3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1af3-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1af3-123">Accept</span></span>|<span data-ttu-id="a1af3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a1af3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1af3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1af3-125">Request body</span></span>
<span data-ttu-id="a1af3-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1af3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1af3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1af3-127">Response</span></span>
<span data-ttu-id="a1af3-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1af3-128">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1af3-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1af3-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1af3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1af3-130">Request</span></span>
<span data-ttu-id="a1af3-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1af3-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="a1af3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1af3-132">Response</span></span>
<span data-ttu-id="a1af3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1af3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 862

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "id": "0e064997-4997-0e06-9749-060e9749060e",
      "version": "Version value"
    }
  ]
}
```




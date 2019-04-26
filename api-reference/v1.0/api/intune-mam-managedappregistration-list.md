---
title: Listar managedAppRegistrations
description: Listar propriedades e relações dos objetos managedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94738c4b0aef555a536ceec2533db241007251a4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553852"
---
# <a name="list-managedappregistrations"></a><span data-ttu-id="c14fb-103">Listar managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="c14fb-103">List managedAppRegistrations</span></span>

> <span data-ttu-id="c14fb-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c14fb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c14fb-105">Listar propriedades e relações dos objetos [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c14fb-105">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c14fb-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c14fb-106">Prerequisites</span></span>
<span data-ttu-id="c14fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c14fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c14fb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c14fb-109">Permission type</span></span>|<span data-ttu-id="c14fb-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c14fb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c14fb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c14fb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c14fb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c14fb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c14fb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c14fb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c14fb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c14fb-114">Not supported.</span></span>|
|<span data-ttu-id="c14fb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c14fb-115">Application</span></span>|<span data-ttu-id="c14fb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c14fb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c14fb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c14fb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="c14fb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c14fb-118">Request headers</span></span>
|<span data-ttu-id="c14fb-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c14fb-119">Header</span></span>|<span data-ttu-id="c14fb-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c14fb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c14fb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c14fb-121">Authorization</span></span>|<span data-ttu-id="c14fb-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c14fb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c14fb-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c14fb-123">Accept</span></span>|<span data-ttu-id="c14fb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c14fb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c14fb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c14fb-125">Request body</span></span>
<span data-ttu-id="c14fb-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c14fb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c14fb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c14fb-127">Response</span></span>
<span data-ttu-id="c14fb-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppRegistration](../resources/intune-mam-managedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c14fb-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c14fb-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c14fb-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c14fb-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c14fb-130">Request</span></span>
<span data-ttu-id="c14fb-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c14fb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="c14fb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c14fb-132">Response</span></span>
<span data-ttu-id="c14fb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c14fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 806

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppRegistration",
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
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "5496aa60-aa60-5496-60aa-965460aa9654",
      "version": "Version value"
    }
  ]
}
```




---
title: Listar mobileAppInstallStatuses
description: Listar Propriedades e relações dos objetos mobileAppInstallStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3eb35d826fff74b853ca7b5d7d4abc2e88c54248
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807522"
---
# <a name="list-mobileappinstallstatuses"></a><span data-ttu-id="77947-103">Listar mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="77947-103">List mobileAppInstallStatuses</span></span>

> <span data-ttu-id="77947-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="77947-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77947-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77947-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77947-106">Listar Propriedades e relações dos objetos [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="77947-106">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77947-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="77947-107">Prerequisites</span></span>
<span data-ttu-id="77947-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77947-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77947-110">Permission type</span></span>|<span data-ttu-id="77947-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="77947-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77947-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77947-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77947-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="77947-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="77947-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77947-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77947-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77947-115">Not supported.</span></span>|
|<span data-ttu-id="77947-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77947-116">Application</span></span>|<span data-ttu-id="77947-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77947-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77947-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77947-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="77947-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77947-119">Request headers</span></span>
|<span data-ttu-id="77947-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77947-120">Header</span></span>|<span data-ttu-id="77947-121">Valor</span><span class="sxs-lookup"><span data-stu-id="77947-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77947-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="77947-122">Authorization</span></span>|<span data-ttu-id="77947-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77947-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77947-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="77947-124">Accept</span></span>|<span data-ttu-id="77947-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77947-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77947-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77947-126">Request body</span></span>
<span data-ttu-id="77947-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="77947-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77947-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="77947-128">Response</span></span>
<span data-ttu-id="77947-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77947-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77947-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77947-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="77947-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77947-131">Request</span></span>
<span data-ttu-id="77947-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77947-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="77947-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="77947-133">Response</span></span>
<span data-ttu-id="77947-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77947-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 693

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
      "id": "7560ee45-ee45-7560-45ee-607545ee6075",
      "deviceName": "Device Name value",
      "deviceId": "Device Id value",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "mobileAppInstallStatusValue": "failed",
      "installState": "failed",
      "installStateDetail": "dependencyFailedToInstall",
      "errorCode": 9,
      "osVersion": "Os Version value",
      "osDescription": "Os Description value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "displayVersion": "Display Version value"
    }
  ]
}
```






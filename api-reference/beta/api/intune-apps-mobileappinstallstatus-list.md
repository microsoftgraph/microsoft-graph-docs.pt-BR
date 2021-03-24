---
title: Listar mobileAppInstallStatuses
description: Listar propriedades e relações dos objetos mobileAppInstallStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: caee4189e113932b287db07ee4de69892a82ea39
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139696"
---
# <a name="list-mobileappinstallstatuses"></a><span data-ttu-id="51caa-103">Listar mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="51caa-103">List mobileAppInstallStatuses</span></span>

<span data-ttu-id="51caa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51caa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51caa-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="51caa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51caa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51caa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51caa-107">Listar propriedades e relações dos objetos [mobileAppInstallStatus.](../resources/intune-apps-mobileappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="51caa-107">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51caa-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51caa-108">Prerequisites</span></span>
<span data-ttu-id="51caa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51caa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51caa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51caa-111">Permission type</span></span>|<span data-ttu-id="51caa-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51caa-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51caa-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51caa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51caa-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51caa-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51caa-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51caa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51caa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51caa-116">Not supported.</span></span>|
|<span data-ttu-id="51caa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51caa-117">Application</span></span>|<span data-ttu-id="51caa-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51caa-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51caa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51caa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="51caa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51caa-120">Request headers</span></span>
|<span data-ttu-id="51caa-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51caa-121">Header</span></span>|<span data-ttu-id="51caa-122">Valor</span><span class="sxs-lookup"><span data-stu-id="51caa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51caa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="51caa-123">Authorization</span></span>|<span data-ttu-id="51caa-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51caa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51caa-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51caa-125">Accept</span></span>|<span data-ttu-id="51caa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51caa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51caa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51caa-127">Request body</span></span>
<span data-ttu-id="51caa-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51caa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51caa-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="51caa-129">Response</span></span>
<span data-ttu-id="51caa-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51caa-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51caa-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51caa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="51caa-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51caa-132">Request</span></span>
<span data-ttu-id="51caa-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51caa-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="51caa-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="51caa-134">Response</span></span>
<span data-ttu-id="51caa-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51caa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





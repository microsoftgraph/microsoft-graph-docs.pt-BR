---
title: Obter mobileAppInstallStatus
description: Leia as propriedades e as relações do objeto mobileAppInstallStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 333f622821f44fcf5387eb243ada4f3287b01f53
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761220"
---
# <a name="get-mobileappinstallstatus"></a><span data-ttu-id="e8ced-103">Obter mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e8ced-103">Get mobileAppInstallStatus</span></span>

> <span data-ttu-id="e8ced-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8ced-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8ced-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8ced-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8ced-106">Leia as propriedades e as relações do objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="e8ced-106">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8ced-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8ced-107">Prerequisites</span></span>
<span data-ttu-id="e8ced-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8ced-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8ced-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8ced-110">Permission type</span></span>|<span data-ttu-id="e8ced-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8ced-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8ced-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8ced-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8ced-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8ced-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e8ced-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8ced-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8ced-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8ced-115">Not supported.</span></span>|
|<span data-ttu-id="e8ced-116">Application</span><span class="sxs-lookup"><span data-stu-id="e8ced-116">Application</span></span>|<span data-ttu-id="e8ced-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8ced-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8ced-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8ced-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8ced-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8ced-119">Optional query parameters</span></span>
<span data-ttu-id="e8ced-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8ced-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8ced-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8ced-121">Request headers</span></span>
|<span data-ttu-id="e8ced-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8ced-122">Header</span></span>|<span data-ttu-id="e8ced-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e8ced-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8ced-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8ced-124">Authorization</span></span>|<span data-ttu-id="e8ced-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8ced-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8ced-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8ced-126">Accept</span></span>|<span data-ttu-id="e8ced-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e8ced-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8ced-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8ced-128">Request body</span></span>
<span data-ttu-id="e8ced-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8ced-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8ced-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8ced-130">Response</span></span>
<span data-ttu-id="e8ced-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8ced-131">If successful, this method returns a `200 OK` response code and [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8ced-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8ced-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8ced-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8ced-133">Request</span></span>
<span data-ttu-id="e8ced-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8ced-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
```

### <a name="response"></a><span data-ttu-id="e8ced-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8ced-135">Response</span></span>
<span data-ttu-id="e8ced-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8ced-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "value": {
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
}
```





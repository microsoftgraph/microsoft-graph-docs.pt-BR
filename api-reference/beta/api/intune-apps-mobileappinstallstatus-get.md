---
title: Obter mobileAppInstallStatus
description: Leia propriedades e relações do objeto mobileAppInstallStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 04bd8f0cf872a9f4bca34bf76cfcb27eb013a167
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143161"
---
# <a name="get-mobileappinstallstatus"></a><span data-ttu-id="40ade-103">Obter mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="40ade-103">Get mobileAppInstallStatus</span></span>

<span data-ttu-id="40ade-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40ade-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40ade-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40ade-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40ade-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40ade-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40ade-107">Leia propriedades e relações do [objeto mobileAppInstallStatus.](../resources/intune-apps-mobileappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="40ade-107">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40ade-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40ade-108">Prerequisites</span></span>
<span data-ttu-id="40ade-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40ade-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40ade-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40ade-111">Permission type</span></span>|<span data-ttu-id="40ade-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40ade-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40ade-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40ade-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40ade-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40ade-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="40ade-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40ade-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40ade-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40ade-116">Not supported.</span></span>|
|<span data-ttu-id="40ade-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40ade-117">Application</span></span>|<span data-ttu-id="40ade-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40ade-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40ade-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40ade-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40ade-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="40ade-120">Optional query parameters</span></span>
<span data-ttu-id="40ade-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="40ade-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40ade-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40ade-122">Request headers</span></span>
|<span data-ttu-id="40ade-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40ade-123">Header</span></span>|<span data-ttu-id="40ade-124">Valor</span><span class="sxs-lookup"><span data-stu-id="40ade-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40ade-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="40ade-125">Authorization</span></span>|<span data-ttu-id="40ade-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40ade-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40ade-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="40ade-127">Accept</span></span>|<span data-ttu-id="40ade-128">application/json</span><span class="sxs-lookup"><span data-stu-id="40ade-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40ade-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40ade-129">Request body</span></span>
<span data-ttu-id="40ade-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40ade-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40ade-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="40ade-131">Response</span></span>
<span data-ttu-id="40ade-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40ade-132">If successful, this method returns a `200 OK` response code and [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40ade-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40ade-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="40ade-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40ade-134">Request</span></span>
<span data-ttu-id="40ade-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40ade-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
```

### <a name="response"></a><span data-ttu-id="40ade-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="40ade-136">Response</span></span>
<span data-ttu-id="40ade-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40ade-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





---
title: Obter userAppInstallStatus
description: Leia as propriedades e as relações do objeto userAppInstallStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94c8249b24fe30421b69079b71a018bf7548a4d0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934912"
---
# <a name="get-userappinstallstatus"></a><span data-ttu-id="abe43-103">Obter userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="abe43-103">Get userAppInstallStatus</span></span>

> <span data-ttu-id="abe43-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="abe43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abe43-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="abe43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abe43-106">Leia as propriedades e as relações do objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="abe43-106">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abe43-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abe43-107">Prerequisites</span></span>
<span data-ttu-id="abe43-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abe43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abe43-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abe43-110">Permission type</span></span>|<span data-ttu-id="abe43-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="abe43-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abe43-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abe43-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abe43-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="abe43-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="abe43-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abe43-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abe43-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abe43-115">Not supported.</span></span>|
|<span data-ttu-id="abe43-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abe43-116">Application</span></span>|<span data-ttu-id="abe43-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abe43-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abe43-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abe43-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abe43-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="abe43-119">Optional query parameters</span></span>
<span data-ttu-id="abe43-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="abe43-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="abe43-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abe43-121">Request headers</span></span>
|<span data-ttu-id="abe43-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abe43-122">Header</span></span>|<span data-ttu-id="abe43-123">Valor</span><span class="sxs-lookup"><span data-stu-id="abe43-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abe43-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="abe43-124">Authorization</span></span>|<span data-ttu-id="abe43-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abe43-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abe43-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="abe43-126">Accept</span></span>|<span data-ttu-id="abe43-127">application/json</span><span class="sxs-lookup"><span data-stu-id="abe43-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abe43-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abe43-128">Request body</span></span>
<span data-ttu-id="abe43-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="abe43-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abe43-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="abe43-130">Response</span></span>
<span data-ttu-id="abe43-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abe43-131">If successful, this method returns a `200 OK` response code and [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abe43-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abe43-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="abe43-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abe43-133">Request</span></span>
<span data-ttu-id="abe43-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abe43-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

### <a name="response"></a><span data-ttu-id="abe43-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="abe43-135">Response</span></span>
<span data-ttu-id="abe43-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abe43-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 321

{
  "value": {
    "@odata.type": "#microsoft.graph.userAppInstallStatus",
    "id": "14959a2a-9a2a-1495-2a9a-95142a9a9514",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7
  }
}
```





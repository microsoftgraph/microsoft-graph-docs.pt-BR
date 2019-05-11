---
title: Listar userAppInstallStatuses
description: Listar Propriedades e relações dos objetos userAppInstallStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e9ddb8be8215e423d9a6bc2219c2180809b8628
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934880"
---
# <a name="list-userappinstallstatuses"></a><span data-ttu-id="277ce-103">Listar userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="277ce-103">List userAppInstallStatuses</span></span>

> <span data-ttu-id="277ce-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="277ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="277ce-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="277ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="277ce-106">Listar Propriedades e relações dos objetos [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="277ce-106">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="277ce-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="277ce-107">Prerequisites</span></span>
<span data-ttu-id="277ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="277ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="277ce-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="277ce-110">Permission type</span></span>|<span data-ttu-id="277ce-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="277ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="277ce-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="277ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="277ce-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="277ce-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="277ce-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="277ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="277ce-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="277ce-115">Not supported.</span></span>|
|<span data-ttu-id="277ce-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="277ce-116">Application</span></span>|<span data-ttu-id="277ce-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="277ce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="277ce-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="277ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="277ce-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="277ce-119">Request headers</span></span>
|<span data-ttu-id="277ce-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="277ce-120">Header</span></span>|<span data-ttu-id="277ce-121">Valor</span><span class="sxs-lookup"><span data-stu-id="277ce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="277ce-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="277ce-122">Authorization</span></span>|<span data-ttu-id="277ce-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="277ce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="277ce-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="277ce-124">Accept</span></span>|<span data-ttu-id="277ce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="277ce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="277ce-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="277ce-126">Request body</span></span>
<span data-ttu-id="277ce-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="277ce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="277ce-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="277ce-128">Response</span></span>
<span data-ttu-id="277ce-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="277ce-129">If successful, this method returns a `200 OK` response code and a collection of [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="277ce-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="277ce-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="277ce-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="277ce-131">Request</span></span>
<span data-ttu-id="277ce-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="277ce-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="277ce-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="277ce-133">Response</span></span>
<span data-ttu-id="277ce-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="277ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userAppInstallStatus",
      "id": "14959a2a-9a2a-1495-2a9a-95142a9a9514",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "installedDeviceCount": 4,
      "failedDeviceCount": 1,
      "notInstalledDeviceCount": 7
    }
  ]
}
```





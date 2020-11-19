---
title: Listar userAppInstallStatuses
description: Listar Propriedades e relações dos objetos userAppInstallStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0827e74e1c92432868c5f4cb23fe79f6c6e8c327
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49247556"
---
# <a name="list-userappinstallstatuses"></a><span data-ttu-id="6e168-103">Listar userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="6e168-103">List userAppInstallStatuses</span></span>

<span data-ttu-id="6e168-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e168-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e168-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e168-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e168-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e168-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e168-107">Listar Propriedades e relações dos objetos [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="6e168-107">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e168-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e168-108">Prerequisites</span></span>
<span data-ttu-id="6e168-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e168-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e168-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e168-111">Permission type</span></span>|<span data-ttu-id="6e168-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6e168-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e168-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e168-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e168-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e168-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6e168-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e168-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e168-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e168-116">Not supported.</span></span>|
|<span data-ttu-id="6e168-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e168-117">Application</span></span>|<span data-ttu-id="6e168-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e168-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e168-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e168-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="6e168-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e168-120">Request headers</span></span>
|<span data-ttu-id="6e168-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e168-121">Header</span></span>|<span data-ttu-id="6e168-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6e168-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e168-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e168-123">Authorization</span></span>|<span data-ttu-id="6e168-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e168-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e168-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6e168-125">Accept</span></span>|<span data-ttu-id="6e168-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e168-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e168-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e168-127">Request body</span></span>
<span data-ttu-id="6e168-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e168-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e168-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e168-129">Response</span></span>
<span data-ttu-id="6e168-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e168-130">If successful, this method returns a `200 OK` response code and a collection of [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e168-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e168-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e168-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e168-132">Request</span></span>
<span data-ttu-id="6e168-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e168-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="6e168-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e168-134">Response</span></span>
<span data-ttu-id="6e168-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e168-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





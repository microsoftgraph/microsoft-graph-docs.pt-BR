---
title: Listar microsoftStoreForBusinessContainedApps
description: Listar Propriedades e relações dos objetos microsoftStoreForBusinessContainedApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1cdc3a60fdd5fa94cea6ceb28e8830cab58b634
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36336807"
---
# <a name="list-microsoftstoreforbusinesscontainedapps"></a><span data-ttu-id="308f8-103">Listar microsoftStoreForBusinessContainedApps</span><span class="sxs-lookup"><span data-stu-id="308f8-103">List microsoftStoreForBusinessContainedApps</span></span>

> <span data-ttu-id="308f8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="308f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="308f8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="308f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="308f8-106">Listar Propriedades e relações dos objetos [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="308f8-106">List properties and relationships of the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="308f8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="308f8-107">Prerequisites</span></span>
<span data-ttu-id="308f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="308f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="308f8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="308f8-110">Permission type</span></span>|<span data-ttu-id="308f8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="308f8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="308f8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="308f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="308f8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="308f8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="308f8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="308f8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="308f8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="308f8-115">Not supported.</span></span>|
|<span data-ttu-id="308f8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="308f8-116">Application</span></span>|<span data-ttu-id="308f8-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="308f8-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="308f8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="308f8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="308f8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="308f8-119">Request headers</span></span>
|<span data-ttu-id="308f8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="308f8-120">Header</span></span>|<span data-ttu-id="308f8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="308f8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="308f8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="308f8-122">Authorization</span></span>|<span data-ttu-id="308f8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="308f8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="308f8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="308f8-124">Accept</span></span>|<span data-ttu-id="308f8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="308f8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="308f8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="308f8-126">Request body</span></span>
<span data-ttu-id="308f8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="308f8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="308f8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="308f8-128">Response</span></span>
<span data-ttu-id="308f8-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="308f8-129">If successful, this method returns a `200 OK` response code and a collection of [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="308f8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="308f8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="308f8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="308f8-131">Request</span></span>
<span data-ttu-id="308f8-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="308f8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
```

### <a name="response"></a><span data-ttu-id="308f8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="308f8-133">Response</span></span>
<span data-ttu-id="308f8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="308f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
      "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
      "appUserModelId": "App User Model Id value"
    }
  ]
}
```







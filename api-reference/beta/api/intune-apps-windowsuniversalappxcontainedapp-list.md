---
title: Listar windowsUniversalAppXContainedApps
description: Listar Propriedades e relações dos objetos windowsUniversalAppXContainedApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f428ff1d57c82147d3b80af682576a99fd40947f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760624"
---
# <a name="list-windowsuniversalappxcontainedapps"></a><span data-ttu-id="6d235-103">Listar windowsUniversalAppXContainedApps</span><span class="sxs-lookup"><span data-stu-id="6d235-103">List windowsUniversalAppXContainedApps</span></span>

> <span data-ttu-id="6d235-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d235-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d235-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d235-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d235-106">Listar Propriedades e relações dos objetos [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="6d235-106">List properties and relationships of the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d235-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6d235-107">Prerequisites</span></span>
<span data-ttu-id="6d235-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d235-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d235-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d235-110">Permission type</span></span>|<span data-ttu-id="6d235-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6d235-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d235-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d235-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6d235-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d235-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6d235-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d235-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d235-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d235-115">Not supported.</span></span>|
|<span data-ttu-id="6d235-116">Application</span><span class="sxs-lookup"><span data-stu-id="6d235-116">Application</span></span>|<span data-ttu-id="6d235-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d235-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d235-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d235-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="6d235-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d235-119">Request headers</span></span>
|<span data-ttu-id="6d235-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d235-120">Header</span></span>|<span data-ttu-id="6d235-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6d235-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d235-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d235-122">Authorization</span></span>|<span data-ttu-id="6d235-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d235-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d235-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d235-124">Accept</span></span>|<span data-ttu-id="6d235-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6d235-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d235-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d235-126">Request body</span></span>
<span data-ttu-id="6d235-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d235-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d235-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d235-128">Response</span></span>
<span data-ttu-id="6d235-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d235-129">If successful, this method returns a `200 OK` response code and a collection of [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d235-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d235-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d235-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d235-131">Request</span></span>
<span data-ttu-id="6d235-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d235-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
```

### <a name="response"></a><span data-ttu-id="6d235-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d235-133">Response</span></span>
<span data-ttu-id="6d235-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d235-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 216

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
      "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
      "appUserModelId": "App User Model Id value"
    }
  ]
}
```





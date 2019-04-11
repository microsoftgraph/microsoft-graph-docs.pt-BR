---
title: Listar windowsUniversalAppXContainedApps
description: Listar Propriedades e relações dos objetos windowsUniversalAppXContainedApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d318265dd4a21ca94a435b90bf12c7a5eba513ba
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31793473"
---
# <a name="list-windowsuniversalappxcontainedapps"></a><span data-ttu-id="99825-103">Listar windowsUniversalAppXContainedApps</span><span class="sxs-lookup"><span data-stu-id="99825-103">List windowsUniversalAppXContainedApps</span></span>

> <span data-ttu-id="99825-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99825-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99825-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99825-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99825-106">Listar Propriedades e relações dos objetos [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="99825-106">List properties and relationships of the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99825-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99825-107">Prerequisites</span></span>
<span data-ttu-id="99825-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99825-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99825-110">Permission type</span></span>|<span data-ttu-id="99825-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="99825-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99825-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99825-112">Delegated (work or school account)</span></span>|<span data-ttu-id="99825-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="99825-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="99825-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99825-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99825-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99825-115">Not supported.</span></span>|
|<span data-ttu-id="99825-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99825-116">Application</span></span>|<span data-ttu-id="99825-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99825-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99825-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99825-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="99825-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99825-119">Request headers</span></span>
|<span data-ttu-id="99825-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99825-120">Header</span></span>|<span data-ttu-id="99825-121">Valor</span><span class="sxs-lookup"><span data-stu-id="99825-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99825-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="99825-122">Authorization</span></span>|<span data-ttu-id="99825-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99825-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99825-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="99825-124">Accept</span></span>|<span data-ttu-id="99825-125">application/json</span><span class="sxs-lookup"><span data-stu-id="99825-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99825-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99825-126">Request body</span></span>
<span data-ttu-id="99825-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99825-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99825-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="99825-128">Response</span></span>
<span data-ttu-id="99825-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99825-129">If successful, this method returns a `200 OK` response code and a collection of [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99825-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99825-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="99825-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99825-131">Request</span></span>
<span data-ttu-id="99825-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99825-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
```

### <a name="response"></a><span data-ttu-id="99825-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="99825-133">Response</span></span>
<span data-ttu-id="99825-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99825-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






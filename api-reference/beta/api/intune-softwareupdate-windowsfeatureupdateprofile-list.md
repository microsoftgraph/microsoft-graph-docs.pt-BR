---
title: Listar windowsFeatureUpdateProfiles
description: Listar Propriedades e relações dos objetos windowsFeatureUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9657a20b42939dfc3fca8e47669e6b8e43225926
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123600"
---
# <a name="list-windowsfeatureupdateprofiles"></a><span data-ttu-id="3ec9c-103">Listar windowsFeatureUpdateProfiles</span><span class="sxs-lookup"><span data-stu-id="3ec9c-103">List windowsFeatureUpdateProfiles</span></span>

<span data-ttu-id="3ec9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ec9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ec9c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3ec9c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ec9c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ec9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ec9c-107">Listar Propriedades e relações dos objetos [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3ec9c-107">List properties and relationships of the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ec9c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3ec9c-108">Prerequisites</span></span>
<span data-ttu-id="3ec9c-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3ec9c-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3ec9c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ec9c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ec9c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ec9c-111">Permission type</span></span>|<span data-ttu-id="3ec9c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3ec9c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ec9c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ec9c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ec9c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec9c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3ec9c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ec9c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ec9c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ec9c-116">Not supported.</span></span>|
|<span data-ttu-id="3ec9c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ec9c-117">Application</span></span>|<span data-ttu-id="3ec9c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec9c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ec9c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ec9c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsFeatureUpdateProfiles
```

## <a name="request-headers"></a><span data-ttu-id="3ec9c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ec9c-120">Request headers</span></span>
|<span data-ttu-id="3ec9c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3ec9c-121">Header</span></span>|<span data-ttu-id="3ec9c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3ec9c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ec9c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ec9c-123">Authorization</span></span>|<span data-ttu-id="3ec9c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ec9c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ec9c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3ec9c-125">Accept</span></span>|<span data-ttu-id="3ec9c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ec9c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ec9c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ec9c-127">Request body</span></span>
<span data-ttu-id="3ec9c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ec9c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ec9c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ec9c-129">Response</span></span>
<span data-ttu-id="3ec9c-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ec9c-130">If successful, this method returns a `200 OK` response code and a collection of [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ec9c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ec9c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ec9c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ec9c-132">Request</span></span>
<span data-ttu-id="3ec9c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ec9c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles
```

### <a name="response"></a><span data-ttu-id="3ec9c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ec9c-134">Response</span></span>
<span data-ttu-id="3ec9c-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="3ec9c-135">Here is an example of the response.</span></span> <span data-ttu-id="3ec9c-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="3ec9c-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3ec9c-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3ec9c-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 514

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
      "id": "885bd4ee-d4ee-885b-eed4-5b88eed45b88",
      "displayName": "Display Name value",
      "description": "Description value",
      "featureUpdateVersion": "Feature Update Version value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




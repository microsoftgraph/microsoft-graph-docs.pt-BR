---
title: Listar windowsFeatureUpdateProfiles
description: Listar Propriedades e relações dos objetos windowsFeatureUpdateProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8413ed39595064762d113df98860937fcfae7a98
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800379"
---
# <a name="list-windowsfeatureupdateprofiles"></a><span data-ttu-id="c84bf-103">Listar windowsFeatureUpdateProfiles</span><span class="sxs-lookup"><span data-stu-id="c84bf-103">List windowsFeatureUpdateProfiles</span></span>

> <span data-ttu-id="c84bf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c84bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c84bf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c84bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c84bf-106">Listar Propriedades e relações dos objetos [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c84bf-106">List properties and relationships of the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c84bf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c84bf-107">Prerequisites</span></span>
<span data-ttu-id="c84bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c84bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c84bf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c84bf-110">Permission type</span></span>|<span data-ttu-id="c84bf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c84bf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c84bf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c84bf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c84bf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c84bf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c84bf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c84bf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c84bf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c84bf-115">Not supported.</span></span>|
|<span data-ttu-id="c84bf-116">Application</span><span class="sxs-lookup"><span data-stu-id="c84bf-116">Application</span></span>|<span data-ttu-id="c84bf-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c84bf-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c84bf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c84bf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsFeatureUpdateProfiles
```

## <a name="request-headers"></a><span data-ttu-id="c84bf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c84bf-119">Request headers</span></span>
|<span data-ttu-id="c84bf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c84bf-120">Header</span></span>|<span data-ttu-id="c84bf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c84bf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c84bf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c84bf-122">Authorization</span></span>|<span data-ttu-id="c84bf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c84bf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c84bf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c84bf-124">Accept</span></span>|<span data-ttu-id="c84bf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c84bf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c84bf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c84bf-126">Request body</span></span>
<span data-ttu-id="c84bf-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c84bf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c84bf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c84bf-128">Response</span></span>
<span data-ttu-id="c84bf-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c84bf-129">If successful, this method returns a `200 OK` response code and a collection of [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c84bf-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c84bf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c84bf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c84bf-131">Request</span></span>
<span data-ttu-id="c84bf-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c84bf-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles
```

### <a name="response"></a><span data-ttu-id="c84bf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c84bf-133">Response</span></span>
<span data-ttu-id="c84bf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c84bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
      "id": "885bd4ee-d4ee-885b-eed4-5b88eed45b88",
      "displayName": "Display Name value",
      "description": "Description value",
      "featureUpdateVersion": "Feature Update Version value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```





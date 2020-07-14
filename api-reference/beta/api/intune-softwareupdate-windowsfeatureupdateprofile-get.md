---
title: Obter windowsFeatureUpdateProfile
description: Leia as propriedades e as relações do objeto windowsFeatureUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 459c61da0b63692877e94557268b54a55ce59951
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123607"
---
# <a name="get-windowsfeatureupdateprofile"></a><span data-ttu-id="f6f10-103">Obter windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="f6f10-103">Get windowsFeatureUpdateProfile</span></span>

<span data-ttu-id="f6f10-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6f10-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6f10-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f6f10-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6f10-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6f10-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6f10-107">Leia as propriedades e as relações do objeto [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f6f10-107">Read properties and relationships of the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6f10-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f6f10-108">Prerequisites</span></span>
<span data-ttu-id="f6f10-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f6f10-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f6f10-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6f10-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6f10-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6f10-111">Permission type</span></span>|<span data-ttu-id="f6f10-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f6f10-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6f10-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6f10-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6f10-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6f10-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f6f10-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6f10-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6f10-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6f10-116">Not supported.</span></span>|
|<span data-ttu-id="f6f10-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6f10-117">Application</span></span>|<span data-ttu-id="f6f10-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6f10-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6f10-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6f10-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6f10-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f6f10-120">Optional query parameters</span></span>
<span data-ttu-id="f6f10-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f6f10-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6f10-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6f10-122">Request headers</span></span>
|<span data-ttu-id="f6f10-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f6f10-123">Header</span></span>|<span data-ttu-id="f6f10-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f6f10-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6f10-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6f10-125">Authorization</span></span>|<span data-ttu-id="f6f10-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6f10-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6f10-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f6f10-127">Accept</span></span>|<span data-ttu-id="f6f10-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f6f10-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6f10-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6f10-129">Request body</span></span>
<span data-ttu-id="f6f10-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f6f10-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6f10-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6f10-131">Response</span></span>
<span data-ttu-id="f6f10-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6f10-132">If successful, this method returns a `200 OK` response code and [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6f10-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6f10-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6f10-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6f10-134">Request</span></span>
<span data-ttu-id="f6f10-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6f10-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

### <a name="response"></a><span data-ttu-id="f6f10-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6f10-136">Response</span></span>
<span data-ttu-id="f6f10-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="f6f10-137">Here is an example of the response.</span></span> <span data-ttu-id="f6f10-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="f6f10-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f6f10-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f6f10-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 480

{
  "value": {
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
}
```




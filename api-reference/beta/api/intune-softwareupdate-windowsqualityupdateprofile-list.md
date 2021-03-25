---
title: Listar windowsQualityUpdateProfiles
description: Listar propriedades e relações dos objetos windowsQualityUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b759e10fe5628fb0398b5797d38fef130580625b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156181"
---
# <a name="list-windowsqualityupdateprofiles"></a><span data-ttu-id="20cea-103">Listar windowsQualityUpdateProfiles</span><span class="sxs-lookup"><span data-stu-id="20cea-103">List windowsQualityUpdateProfiles</span></span>

<span data-ttu-id="20cea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20cea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20cea-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="20cea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20cea-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20cea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20cea-107">Listar propriedades e relações dos objetos [windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20cea-107">List properties and relationships of the [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20cea-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="20cea-108">Prerequisites</span></span>
<span data-ttu-id="20cea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20cea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20cea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20cea-111">Permission type</span></span>|<span data-ttu-id="20cea-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20cea-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20cea-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20cea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20cea-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20cea-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="20cea-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20cea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20cea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20cea-116">Not supported.</span></span>|
|<span data-ttu-id="20cea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20cea-117">Application</span></span>|<span data-ttu-id="20cea-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20cea-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20cea-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20cea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsQualityUpdateProfiles
```

## <a name="request-headers"></a><span data-ttu-id="20cea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20cea-120">Request headers</span></span>
|<span data-ttu-id="20cea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20cea-121">Header</span></span>|<span data-ttu-id="20cea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="20cea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20cea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="20cea-123">Authorization</span></span>|<span data-ttu-id="20cea-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20cea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20cea-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="20cea-125">Accept</span></span>|<span data-ttu-id="20cea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20cea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20cea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20cea-127">Request body</span></span>
<span data-ttu-id="20cea-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20cea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20cea-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="20cea-129">Response</span></span>
<span data-ttu-id="20cea-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20cea-130">If successful, this method returns a `200 OK` response code and a collection of [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20cea-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20cea-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="20cea-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20cea-132">Request</span></span>
<span data-ttu-id="20cea-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20cea-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles
```

### <a name="response"></a><span data-ttu-id="20cea-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="20cea-134">Response</span></span>
<span data-ttu-id="20cea-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20cea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 827

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsQualityUpdateProfile",
      "id": "76fc7b65-7b65-76fc-657b-fc76657bfc76",
      "displayName": "Display Name value",
      "description": "Description value",
      "expeditedUpdateSettings": {
        "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings",
        "qualityUpdateRelease": "Quality Update Release value",
        "daysUntilForcedReboot": 5
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "releaseDateDisplayName": "Release Date Display Name value",
      "deployableContentDisplayName": "Deployable Content Display Name value"
    }
  ]
}
```





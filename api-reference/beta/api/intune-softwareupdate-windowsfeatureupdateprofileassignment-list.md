---
title: Listar windowsFeatureUpdateProfileAssignments
description: Listar Propriedades e relações dos objetos windowsFeatureUpdateProfileAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 99ce7aaae200e9a88079f7f5f0bb0552663dd4dd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800344"
---
# <a name="list-windowsfeatureupdateprofileassignments"></a><span data-ttu-id="946c1-103">Listar windowsFeatureUpdateProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="946c1-103">List windowsFeatureUpdateProfileAssignments</span></span>

> <span data-ttu-id="946c1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="946c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="946c1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="946c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="946c1-106">Listar Propriedades e relações dos objetos [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="946c1-106">List properties and relationships of the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="946c1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="946c1-107">Prerequisites</span></span>
<span data-ttu-id="946c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="946c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="946c1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="946c1-110">Permission type</span></span>|<span data-ttu-id="946c1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="946c1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="946c1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="946c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="946c1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="946c1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="946c1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="946c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="946c1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="946c1-115">Not supported.</span></span>|
|<span data-ttu-id="946c1-116">Application</span><span class="sxs-lookup"><span data-stu-id="946c1-116">Application</span></span>|<span data-ttu-id="946c1-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="946c1-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="946c1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="946c1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="946c1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="946c1-119">Request headers</span></span>
|<span data-ttu-id="946c1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="946c1-120">Header</span></span>|<span data-ttu-id="946c1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="946c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="946c1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="946c1-122">Authorization</span></span>|<span data-ttu-id="946c1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="946c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="946c1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="946c1-124">Accept</span></span>|<span data-ttu-id="946c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="946c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="946c1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="946c1-126">Request body</span></span>
<span data-ttu-id="946c1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="946c1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="946c1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="946c1-128">Response</span></span>
<span data-ttu-id="946c1-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="946c1-129">If successful, this method returns a `200 OK` response code and a collection of [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="946c1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="946c1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="946c1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="946c1-131">Request</span></span>
<span data-ttu-id="946c1-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="946c1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
```

### <a name="response"></a><span data-ttu-id="946c1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="946c1-133">Response</span></span>
<span data-ttu-id="946c1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="946c1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
      "id": "567a744f-744f-567a-4f74-7a564f747a56",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





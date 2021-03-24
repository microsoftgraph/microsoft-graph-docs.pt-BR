---
title: Listar intuneBrandingProfileAssignments
description: Listar propriedades e relações dos objetos intuneBrandingProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7fa618c8602349b7e13f07ad7c68b1c739e02af7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144918"
---
# <a name="list-intunebrandingprofileassignments"></a><span data-ttu-id="43423-103">Listar intuneBrandingProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="43423-103">List intuneBrandingProfileAssignments</span></span>

<span data-ttu-id="43423-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43423-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43423-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="43423-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43423-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43423-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43423-107">Listar propriedades e relações dos objetos [intuneBrandingProfileAssignment.](../resources/intune-wip-intunebrandingprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="43423-107">List properties and relationships of the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43423-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="43423-108">Prerequisites</span></span>
<span data-ttu-id="43423-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43423-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43423-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43423-111">Permission type</span></span>|<span data-ttu-id="43423-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43423-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43423-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43423-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43423-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43423-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="43423-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43423-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43423-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43423-116">Not supported.</span></span>|
|<span data-ttu-id="43423-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43423-117">Application</span></span>|<span data-ttu-id="43423-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43423-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43423-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43423-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="43423-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43423-120">Request headers</span></span>
|<span data-ttu-id="43423-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43423-121">Header</span></span>|<span data-ttu-id="43423-122">Valor</span><span class="sxs-lookup"><span data-stu-id="43423-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43423-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="43423-123">Authorization</span></span>|<span data-ttu-id="43423-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43423-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43423-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="43423-125">Accept</span></span>|<span data-ttu-id="43423-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43423-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43423-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43423-127">Request body</span></span>
<span data-ttu-id="43423-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43423-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43423-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="43423-129">Response</span></span>
<span data-ttu-id="43423-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43423-130">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43423-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43423-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="43423-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43423-132">Request</span></span>
<span data-ttu-id="43423-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43423-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

### <a name="response"></a><span data-ttu-id="43423-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="43423-134">Response</span></span>
<span data-ttu-id="43423-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43423-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
      "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```





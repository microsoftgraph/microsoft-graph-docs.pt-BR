---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4cfd37a54c29a5f531158984b70afb92da73737b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791234"
---
# <a name="assign-action"></a><span data-ttu-id="d56eb-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="d56eb-103">assign action</span></span>

<span data-ttu-id="d56eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d56eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d56eb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d56eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d56eb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d56eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d56eb-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d56eb-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d56eb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d56eb-108">Prerequisites</span></span>
<span data-ttu-id="d56eb-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d56eb-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d56eb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d56eb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d56eb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d56eb-111">Permission type</span></span>|<span data-ttu-id="d56eb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d56eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d56eb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d56eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d56eb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d56eb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d56eb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d56eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d56eb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d56eb-116">Not supported.</span></span>|
|<span data-ttu-id="d56eb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d56eb-117">Application</span></span>|<span data-ttu-id="d56eb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d56eb-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d56eb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d56eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="d56eb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d56eb-120">Request headers</span></span>
|<span data-ttu-id="d56eb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d56eb-121">Header</span></span>|<span data-ttu-id="d56eb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d56eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d56eb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d56eb-123">Authorization</span></span>|<span data-ttu-id="d56eb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d56eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d56eb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d56eb-125">Accept</span></span>|<span data-ttu-id="d56eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d56eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d56eb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d56eb-127">Request body</span></span>
<span data-ttu-id="d56eb-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d56eb-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d56eb-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d56eb-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d56eb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d56eb-130">Property</span></span>|<span data-ttu-id="d56eb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d56eb-131">Type</span></span>|<span data-ttu-id="d56eb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d56eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d56eb-133">assignments</span><span class="sxs-lookup"><span data-stu-id="d56eb-133">assignments</span></span>|<span data-ttu-id="d56eb-134">coleção [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d56eb-134">[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) collection</span></span>|<span data-ttu-id="d56eb-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d56eb-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d56eb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d56eb-136">Response</span></span>
<span data-ttu-id="d56eb-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d56eb-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d56eb-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d56eb-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d56eb-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d56eb-139">Request</span></span>
<span data-ttu-id="d56eb-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d56eb-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assign

Content-type: application/json
Content-length: 442

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
      "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d56eb-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d56eb-141">Response</span></span>
<span data-ttu-id="d56eb-142">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="d56eb-142">Here is an example of the response.</span></span> <span data-ttu-id="d56eb-143">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="d56eb-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d56eb-144">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="d56eb-144">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




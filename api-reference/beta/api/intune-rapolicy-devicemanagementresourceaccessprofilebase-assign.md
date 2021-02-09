---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7947a3a1c8fb3c315f8e1f60db8b4231b52be8f9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162017"
---
# <a name="assign-action"></a><span data-ttu-id="ed098-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="ed098-103">assign action</span></span>

<span data-ttu-id="ed098-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed098-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed098-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ed098-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed098-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed098-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed098-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ed098-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed098-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed098-108">Prerequisites</span></span>
<span data-ttu-id="ed098-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed098-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed098-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed098-111">Permission type</span></span>|<span data-ttu-id="ed098-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed098-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed098-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed098-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed098-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed098-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ed098-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed098-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed098-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed098-116">Not supported.</span></span>|
|<span data-ttu-id="ed098-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed098-117">Application</span></span>|<span data-ttu-id="ed098-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed098-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed098-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed098-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="ed098-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed098-120">Request headers</span></span>
|<span data-ttu-id="ed098-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed098-121">Header</span></span>|<span data-ttu-id="ed098-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ed098-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed098-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed098-123">Authorization</span></span>|<span data-ttu-id="ed098-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed098-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed098-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed098-125">Accept</span></span>|<span data-ttu-id="ed098-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed098-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed098-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed098-127">Request body</span></span>
<span data-ttu-id="ed098-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ed098-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ed098-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ed098-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ed098-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed098-130">Property</span></span>|<span data-ttu-id="ed098-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed098-131">Type</span></span>|<span data-ttu-id="ed098-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed098-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed098-133">assignments</span><span class="sxs-lookup"><span data-stu-id="ed098-133">assignments</span></span>|<span data-ttu-id="ed098-134">[Coleção deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ed098-134">[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) collection</span></span>|<span data-ttu-id="ed098-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ed098-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ed098-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed098-136">Response</span></span>
<span data-ttu-id="ed098-137">Se tiver êxito, esta ação retornará um código de resposta e uma coleção `200 OK` [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed098-137">If successful, this action returns a `200 OK` response code and a [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed098-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed098-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed098-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed098-139">Request</span></span>
<span data-ttu-id="ed098-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed098-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assign

Content-type: application/json
Content-length: 591

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
      "id": "4ebb8d4e-8d4e-4ebb-4e8d-bb4e4e8dbb4e",
      "intent": "remove",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      },
      "sourceId": "Source Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ed098-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed098-141">Response</span></span>
<span data-ttu-id="ed098-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed098-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 585

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
      "id": "4ebb8d4e-8d4e-4ebb-4e8d-bb4e4e8dbb4e",
      "intent": "remove",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      },
      "sourceId": "Source Id value"
    }
  ]
}
```





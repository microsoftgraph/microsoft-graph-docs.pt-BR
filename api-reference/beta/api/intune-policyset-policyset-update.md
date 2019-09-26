---
title: ação Update
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 79eed9e65e4ba0a5e5ad94d7c882a0128b269041
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191736"
---
# <a name="update-action"></a><span data-ttu-id="27842-103">ação Update</span><span class="sxs-lookup"><span data-stu-id="27842-103">update action</span></span>

> <span data-ttu-id="27842-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="27842-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27842-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27842-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27842-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="27842-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27842-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27842-107">Prerequisites</span></span>
<span data-ttu-id="27842-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27842-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27842-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27842-110">Permission type</span></span>|<span data-ttu-id="27842-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27842-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27842-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27842-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27842-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27842-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27842-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27842-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27842-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27842-115">Not supported.</span></span>|
|<span data-ttu-id="27842-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27842-116">Application</span></span>|<span data-ttu-id="27842-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27842-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27842-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27842-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/update
```

## <a name="request-headers"></a><span data-ttu-id="27842-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27842-119">Request headers</span></span>
|<span data-ttu-id="27842-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27842-120">Header</span></span>|<span data-ttu-id="27842-121">Valor</span><span class="sxs-lookup"><span data-stu-id="27842-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27842-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="27842-122">Authorization</span></span>|<span data-ttu-id="27842-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27842-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27842-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="27842-124">Accept</span></span>|<span data-ttu-id="27842-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27842-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27842-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27842-126">Request body</span></span>
<span data-ttu-id="27842-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="27842-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="27842-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="27842-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="27842-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27842-129">Property</span></span>|<span data-ttu-id="27842-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="27842-130">Type</span></span>|<span data-ttu-id="27842-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="27842-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27842-132">addedPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="27842-132">addedPolicySetItems</span></span>|<span data-ttu-id="27842-133">coleção [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="27842-133">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="27842-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="27842-134">Not yet documented</span></span>|
|<span data-ttu-id="27842-135">updatedPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="27842-135">updatedPolicySetItems</span></span>|<span data-ttu-id="27842-136">coleção [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="27842-136">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="27842-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="27842-137">Not yet documented</span></span>|
|<span data-ttu-id="27842-138">deletedPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="27842-138">deletedPolicySetItems</span></span>|<span data-ttu-id="27842-139">String collection</span><span class="sxs-lookup"><span data-stu-id="27842-139">String collection</span></span>|<span data-ttu-id="27842-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="27842-140">Not yet documented</span></span>|
|<span data-ttu-id="27842-141">assignments</span><span class="sxs-lookup"><span data-stu-id="27842-141">assignments</span></span>|<span data-ttu-id="27842-142">coleção [policySetAssignment](../resources/intune-policyset-policysetassignment.md)</span><span class="sxs-lookup"><span data-stu-id="27842-142">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="27842-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="27842-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="27842-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="27842-144">Response</span></span>
<span data-ttu-id="27842-145">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="27842-145">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="27842-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27842-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="27842-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27842-147">Request</span></span>
<span data-ttu-id="27842-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27842-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/update

Content-type: application/json
Content-length: 1529

{
  "addedPolicySetItems": [
    {
      "@odata.type": "#microsoft.graph.policySetItem",
      "id": "06ec9d5e-9d5e-06ec-5e9d-ec065e9dec06",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "payloadId": "Payload Id value",
      "itemType": "Item Type value",
      "displayName": "Display Name value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ]
    }
  ],
  "updatedPolicySetItems": [
    {
      "@odata.type": "#microsoft.graph.policySetItem",
      "id": "06ec9d5e-9d5e-06ec-5e9d-ec065e9dec06",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "payloadId": "Payload Id value",
      "itemType": "Item Type value",
      "displayName": "Display Name value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ]
    }
  ],
  "deletedPolicySetItems": [
    "Deleted Policy Set Items value"
  ],
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.policySetAssignment",
      "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="27842-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="27842-149">Response</span></span>
<span data-ttu-id="27842-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27842-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





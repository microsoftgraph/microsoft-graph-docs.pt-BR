---
title: ação Update
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 406c27f5e57c0aa4ac68e66ab53d1bdd77b9811b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791718"
---
# <a name="update-action"></a><span data-ttu-id="dcb11-103">ação Update</span><span class="sxs-lookup"><span data-stu-id="dcb11-103">update action</span></span>

<span data-ttu-id="dcb11-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcb11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dcb11-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dcb11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcb11-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dcb11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcb11-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dcb11-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcb11-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dcb11-108">Prerequisites</span></span>
<span data-ttu-id="dcb11-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcb11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcb11-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcb11-111">Permission type</span></span>|<span data-ttu-id="dcb11-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dcb11-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcb11-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcb11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dcb11-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcb11-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dcb11-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcb11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcb11-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcb11-116">Not supported.</span></span>|
|<span data-ttu-id="dcb11-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcb11-117">Application</span></span>|<span data-ttu-id="dcb11-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcb11-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcb11-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcb11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/update
```

## <a name="request-headers"></a><span data-ttu-id="dcb11-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcb11-120">Request headers</span></span>
|<span data-ttu-id="dcb11-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dcb11-121">Header</span></span>|<span data-ttu-id="dcb11-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dcb11-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcb11-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcb11-123">Authorization</span></span>|<span data-ttu-id="dcb11-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcb11-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcb11-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dcb11-125">Accept</span></span>|<span data-ttu-id="dcb11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dcb11-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcb11-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcb11-127">Request body</span></span>
<span data-ttu-id="dcb11-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="dcb11-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dcb11-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="dcb11-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dcb11-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dcb11-130">Property</span></span>|<span data-ttu-id="dcb11-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dcb11-131">Type</span></span>|<span data-ttu-id="dcb11-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcb11-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcb11-133">addedPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="dcb11-133">addedPolicySetItems</span></span>|<span data-ttu-id="dcb11-134">coleção [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dcb11-134">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="dcb11-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dcb11-135">Not yet documented</span></span>|
|<span data-ttu-id="dcb11-136">updatedPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="dcb11-136">updatedPolicySetItems</span></span>|<span data-ttu-id="dcb11-137">coleção [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dcb11-137">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="dcb11-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dcb11-138">Not yet documented</span></span>|
|<span data-ttu-id="dcb11-139">deletedPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="dcb11-139">deletedPolicySetItems</span></span>|<span data-ttu-id="dcb11-140">String collection</span><span class="sxs-lookup"><span data-stu-id="dcb11-140">String collection</span></span>|<span data-ttu-id="dcb11-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dcb11-141">Not yet documented</span></span>|
|<span data-ttu-id="dcb11-142">assignments</span><span class="sxs-lookup"><span data-stu-id="dcb11-142">assignments</span></span>|<span data-ttu-id="dcb11-143">coleção [policySetAssignment](../resources/intune-policyset-policysetassignment.md)</span><span class="sxs-lookup"><span data-stu-id="dcb11-143">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="dcb11-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dcb11-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dcb11-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcb11-145">Response</span></span>
<span data-ttu-id="dcb11-146">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dcb11-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dcb11-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dcb11-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcb11-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcb11-148">Request</span></span>
<span data-ttu-id="dcb11-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcb11-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/update

Content-type: application/json
Content-length: 1692

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="dcb11-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcb11-150">Response</span></span>
<span data-ttu-id="dcb11-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dcb11-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




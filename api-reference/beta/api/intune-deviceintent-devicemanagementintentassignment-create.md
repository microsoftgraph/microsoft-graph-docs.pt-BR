---
title: Criar deviceManagementIntentAssignment
description: Crie um novo objeto deviceManagementIntentAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 86bc4a5efe259190bcab5e7922317f2706bf3992
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128835"
---
# <a name="create-devicemanagementintentassignment"></a><span data-ttu-id="6b632-103">Criar deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="6b632-103">Create deviceManagementIntentAssignment</span></span>

<span data-ttu-id="6b632-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b632-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b632-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b632-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b632-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b632-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b632-107">Crie um novo [objeto deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6b632-107">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b632-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6b632-108">Prerequisites</span></span>
<span data-ttu-id="6b632-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b632-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b632-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b632-111">Permission type</span></span>|<span data-ttu-id="6b632-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b632-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b632-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b632-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b632-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b632-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b632-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b632-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b632-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b632-116">Not supported.</span></span>|
|<span data-ttu-id="6b632-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b632-117">Application</span></span>|<span data-ttu-id="6b632-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b632-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b632-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b632-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6b632-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b632-120">Request headers</span></span>
|<span data-ttu-id="6b632-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b632-121">Header</span></span>|<span data-ttu-id="6b632-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6b632-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b632-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b632-123">Authorization</span></span>|<span data-ttu-id="6b632-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b632-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b632-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6b632-125">Accept</span></span>|<span data-ttu-id="6b632-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b632-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b632-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b632-127">Request body</span></span>
<span data-ttu-id="6b632-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementIntentAssignment.</span><span class="sxs-lookup"><span data-stu-id="6b632-128">In the request body, supply a JSON representation for the deviceManagementIntentAssignment object.</span></span>

<span data-ttu-id="6b632-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntentAssignment.</span><span class="sxs-lookup"><span data-stu-id="6b632-129">The following table shows the properties that are required when you create the deviceManagementIntentAssignment.</span></span>

|<span data-ttu-id="6b632-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b632-130">Property</span></span>|<span data-ttu-id="6b632-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b632-131">Type</span></span>|<span data-ttu-id="6b632-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b632-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b632-133">id</span><span class="sxs-lookup"><span data-stu-id="6b632-133">id</span></span>|<span data-ttu-id="6b632-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b632-134">String</span></span>|<span data-ttu-id="6b632-135">A ID da atribuição</span><span class="sxs-lookup"><span data-stu-id="6b632-135">The assignment ID</span></span>|
|<span data-ttu-id="6b632-136">destino</span><span class="sxs-lookup"><span data-stu-id="6b632-136">target</span></span>|[<span data-ttu-id="6b632-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6b632-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6b632-138">O destino da atribuição</span><span class="sxs-lookup"><span data-stu-id="6b632-138">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="6b632-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b632-139">Response</span></span>
<span data-ttu-id="6b632-140">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b632-140">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b632-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b632-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b632-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b632-142">Request</span></span>
<span data-ttu-id="6b632-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b632-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="6b632-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b632-144">Response</span></span>
<span data-ttu-id="6b632-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b632-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```





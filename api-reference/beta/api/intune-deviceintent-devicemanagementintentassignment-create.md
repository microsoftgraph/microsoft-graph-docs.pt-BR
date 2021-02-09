---
title: Criar deviceManagementIntentAssignment
description: Crie um novo objeto deviceManagementIntentAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e8a9ba1dd1fbaacd1f6b12bb280cc1c5d984ad3
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155157"
---
# <a name="create-devicemanagementintentassignment"></a><span data-ttu-id="77e16-103">Criar deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="77e16-103">Create deviceManagementIntentAssignment</span></span>

<span data-ttu-id="77e16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77e16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77e16-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="77e16-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77e16-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77e16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77e16-107">Crie um novo [objeto deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)</span><span class="sxs-lookup"><span data-stu-id="77e16-107">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77e16-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="77e16-108">Prerequisites</span></span>
<span data-ttu-id="77e16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77e16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77e16-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77e16-111">Permission type</span></span>|<span data-ttu-id="77e16-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="77e16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77e16-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77e16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77e16-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77e16-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77e16-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77e16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77e16-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77e16-116">Not supported.</span></span>|
|<span data-ttu-id="77e16-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77e16-117">Application</span></span>|<span data-ttu-id="77e16-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77e16-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77e16-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77e16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="77e16-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77e16-120">Request headers</span></span>
|<span data-ttu-id="77e16-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77e16-121">Header</span></span>|<span data-ttu-id="77e16-122">Valor</span><span class="sxs-lookup"><span data-stu-id="77e16-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77e16-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="77e16-123">Authorization</span></span>|<span data-ttu-id="77e16-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77e16-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77e16-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="77e16-125">Accept</span></span>|<span data-ttu-id="77e16-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77e16-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77e16-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77e16-127">Request body</span></span>
<span data-ttu-id="77e16-128">No corpo da solicitação, fornece uma representação JSON do objeto deviceManagementIntentAssignment.</span><span class="sxs-lookup"><span data-stu-id="77e16-128">In the request body, supply a JSON representation for the deviceManagementIntentAssignment object.</span></span>

<span data-ttu-id="77e16-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntentAssignment.</span><span class="sxs-lookup"><span data-stu-id="77e16-129">The following table shows the properties that are required when you create the deviceManagementIntentAssignment.</span></span>

|<span data-ttu-id="77e16-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77e16-130">Property</span></span>|<span data-ttu-id="77e16-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="77e16-131">Type</span></span>|<span data-ttu-id="77e16-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="77e16-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77e16-133">id</span><span class="sxs-lookup"><span data-stu-id="77e16-133">id</span></span>|<span data-ttu-id="77e16-134">String</span><span class="sxs-lookup"><span data-stu-id="77e16-134">String</span></span>|<span data-ttu-id="77e16-135">A ID de atribuição</span><span class="sxs-lookup"><span data-stu-id="77e16-135">The assignment ID</span></span>|
|<span data-ttu-id="77e16-136">destino</span><span class="sxs-lookup"><span data-stu-id="77e16-136">target</span></span>|[<span data-ttu-id="77e16-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="77e16-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="77e16-138">O destino da atribuição</span><span class="sxs-lookup"><span data-stu-id="77e16-138">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="77e16-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="77e16-139">Response</span></span>
<span data-ttu-id="77e16-140">Se bem-sucedido, este método retorna um código de resposta e um `201 Created` [objeto deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77e16-140">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77e16-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77e16-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="77e16-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77e16-142">Request</span></span>
<span data-ttu-id="77e16-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77e16-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="77e16-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="77e16-144">Response</span></span>
<span data-ttu-id="77e16-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77e16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





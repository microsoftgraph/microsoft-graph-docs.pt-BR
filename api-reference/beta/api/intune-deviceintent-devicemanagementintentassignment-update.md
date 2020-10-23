---
title: Atualizar deviceManagementIntentAssignment
description: Atualiza as propriedades de um objeto deviceManagementIntentAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f8fc6eecdcefc3081d5673e9d3ed5a1640cd38a6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735530"
---
# <a name="update-devicemanagementintentassignment"></a><span data-ttu-id="287de-103">Atualizar deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="287de-103">Update deviceManagementIntentAssignment</span></span>

<span data-ttu-id="287de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="287de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="287de-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="287de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="287de-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="287de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="287de-107">Atualiza as propriedades de um objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="287de-107">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="287de-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="287de-108">Prerequisites</span></span>
<span data-ttu-id="287de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="287de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="287de-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="287de-111">Permission type</span></span>|<span data-ttu-id="287de-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="287de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="287de-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="287de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="287de-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="287de-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="287de-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="287de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="287de-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="287de-116">Not supported.</span></span>|
|<span data-ttu-id="287de-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="287de-117">Application</span></span>|<span data-ttu-id="287de-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="287de-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="287de-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="287de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="287de-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="287de-120">Request headers</span></span>
|<span data-ttu-id="287de-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="287de-121">Header</span></span>|<span data-ttu-id="287de-122">Valor</span><span class="sxs-lookup"><span data-stu-id="287de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="287de-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="287de-123">Authorization</span></span>|<span data-ttu-id="287de-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="287de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="287de-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="287de-125">Accept</span></span>|<span data-ttu-id="287de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="287de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="287de-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="287de-127">Request body</span></span>
<span data-ttu-id="287de-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="287de-128">In the request body, supply a JSON representation for the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

<span data-ttu-id="287de-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span><span class="sxs-lookup"><span data-stu-id="287de-129">The following table shows the properties that are required when you create the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>

|<span data-ttu-id="287de-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="287de-130">Property</span></span>|<span data-ttu-id="287de-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="287de-131">Type</span></span>|<span data-ttu-id="287de-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="287de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="287de-133">id</span><span class="sxs-lookup"><span data-stu-id="287de-133">id</span></span>|<span data-ttu-id="287de-134">String</span><span class="sxs-lookup"><span data-stu-id="287de-134">String</span></span>|<span data-ttu-id="287de-135">A ID da atribuição</span><span class="sxs-lookup"><span data-stu-id="287de-135">The assignment ID</span></span>|
|<span data-ttu-id="287de-136">destino</span><span class="sxs-lookup"><span data-stu-id="287de-136">target</span></span>|[<span data-ttu-id="287de-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="287de-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="287de-138">O destino da atribuição</span><span class="sxs-lookup"><span data-stu-id="287de-138">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="287de-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="287de-139">Response</span></span>
<span data-ttu-id="287de-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="287de-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="287de-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="287de-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="287de-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="287de-142">Request</span></span>
<span data-ttu-id="287de-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="287de-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
Content-type: application/json
Content-length: 327

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="287de-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="287de-144">Response</span></span>
<span data-ttu-id="287de-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="287de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```






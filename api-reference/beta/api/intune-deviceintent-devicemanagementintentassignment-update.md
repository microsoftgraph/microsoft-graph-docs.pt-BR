---
title: Atualizar deviceManagementIntentAssignment
description: Atualiza as propriedades de um objeto deviceManagementIntentAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a1fd6d161288bc3be0323478ea2d3ac79529397c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42471040"
---
# <a name="update-devicemanagementintentassignment"></a><span data-ttu-id="b89f8-103">Atualizar deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="b89f8-103">Update deviceManagementIntentAssignment</span></span>

<span data-ttu-id="b89f8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b89f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b89f8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b89f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b89f8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b89f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b89f8-107">Atualiza as propriedades de um objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b89f8-107">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b89f8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b89f8-108">Prerequisites</span></span>
<span data-ttu-id="b89f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b89f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b89f8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b89f8-111">Permission type</span></span>|<span data-ttu-id="b89f8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b89f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b89f8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b89f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b89f8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b89f8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b89f8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b89f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b89f8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b89f8-116">Not supported.</span></span>|
|<span data-ttu-id="b89f8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b89f8-117">Application</span></span>|<span data-ttu-id="b89f8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b89f8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b89f8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b89f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b89f8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b89f8-120">Request headers</span></span>
|<span data-ttu-id="b89f8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b89f8-121">Header</span></span>|<span data-ttu-id="b89f8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b89f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b89f8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b89f8-123">Authorization</span></span>|<span data-ttu-id="b89f8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b89f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b89f8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b89f8-125">Accept</span></span>|<span data-ttu-id="b89f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b89f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b89f8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b89f8-127">Request body</span></span>
<span data-ttu-id="b89f8-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b89f8-128">In the request body, supply a JSON representation for the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

<span data-ttu-id="b89f8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b89f8-129">The following table shows the properties that are required when you create the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>

|<span data-ttu-id="b89f8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b89f8-130">Property</span></span>|<span data-ttu-id="b89f8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b89f8-131">Type</span></span>|<span data-ttu-id="b89f8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b89f8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b89f8-133">id</span><span class="sxs-lookup"><span data-stu-id="b89f8-133">id</span></span>|<span data-ttu-id="b89f8-134">String</span><span class="sxs-lookup"><span data-stu-id="b89f8-134">String</span></span>|<span data-ttu-id="b89f8-135">A ID da atribuição</span><span class="sxs-lookup"><span data-stu-id="b89f8-135">The assignment ID</span></span>|
|<span data-ttu-id="b89f8-136">destino</span><span class="sxs-lookup"><span data-stu-id="b89f8-136">target</span></span>|[<span data-ttu-id="b89f8-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b89f8-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b89f8-138">O destino da atribuição</span><span class="sxs-lookup"><span data-stu-id="b89f8-138">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="b89f8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b89f8-139">Response</span></span>
<span data-ttu-id="b89f8-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b89f8-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b89f8-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b89f8-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b89f8-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b89f8-142">Request</span></span>
<span data-ttu-id="b89f8-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b89f8-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b89f8-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b89f8-144">Response</span></span>
<span data-ttu-id="b89f8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b89f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```






---
title: Criar deviceManagementIntentAssignment
description: Criar um novo objeto deviceManagementIntentAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 63eb168a175613fdca7c84559fcd5c368958c446
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792573"
---
# <a name="create-devicemanagementintentassignment"></a><span data-ttu-id="31dad-103">Criar deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="31dad-103">Create deviceManagementIntentAssignment</span></span>

<span data-ttu-id="31dad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31dad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31dad-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="31dad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31dad-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31dad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31dad-107">Criar um novo objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="31dad-107">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31dad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="31dad-108">Prerequisites</span></span>
<span data-ttu-id="31dad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31dad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31dad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31dad-111">Permission type</span></span>|<span data-ttu-id="31dad-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="31dad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31dad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31dad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31dad-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31dad-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="31dad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31dad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31dad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31dad-116">Not supported.</span></span>|
|<span data-ttu-id="31dad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31dad-117">Application</span></span>|<span data-ttu-id="31dad-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31dad-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31dad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31dad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="31dad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31dad-120">Request headers</span></span>
|<span data-ttu-id="31dad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31dad-121">Header</span></span>|<span data-ttu-id="31dad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="31dad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31dad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="31dad-123">Authorization</span></span>|<span data-ttu-id="31dad-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31dad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31dad-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="31dad-125">Accept</span></span>|<span data-ttu-id="31dad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31dad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31dad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31dad-127">Request body</span></span>
<span data-ttu-id="31dad-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementIntentAssignment.</span><span class="sxs-lookup"><span data-stu-id="31dad-128">In the request body, supply a JSON representation for the deviceManagementIntentAssignment object.</span></span>

<span data-ttu-id="31dad-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntentAssignment.</span><span class="sxs-lookup"><span data-stu-id="31dad-129">The following table shows the properties that are required when you create the deviceManagementIntentAssignment.</span></span>

|<span data-ttu-id="31dad-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31dad-130">Property</span></span>|<span data-ttu-id="31dad-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="31dad-131">Type</span></span>|<span data-ttu-id="31dad-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="31dad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31dad-133">id</span><span class="sxs-lookup"><span data-stu-id="31dad-133">id</span></span>|<span data-ttu-id="31dad-134">String</span><span class="sxs-lookup"><span data-stu-id="31dad-134">String</span></span>|<span data-ttu-id="31dad-135">A ID da atribuição</span><span class="sxs-lookup"><span data-stu-id="31dad-135">The assignment ID</span></span>|
|<span data-ttu-id="31dad-136">destino</span><span class="sxs-lookup"><span data-stu-id="31dad-136">target</span></span>|[<span data-ttu-id="31dad-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="31dad-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="31dad-138">O destino da atribuição</span><span class="sxs-lookup"><span data-stu-id="31dad-138">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="31dad-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="31dad-139">Response</span></span>
<span data-ttu-id="31dad-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31dad-140">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31dad-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31dad-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="31dad-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31dad-142">Request</span></span>
<span data-ttu-id="31dad-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31dad-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments
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

### <a name="response"></a><span data-ttu-id="31dad-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="31dad-144">Response</span></span>
<span data-ttu-id="31dad-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31dad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




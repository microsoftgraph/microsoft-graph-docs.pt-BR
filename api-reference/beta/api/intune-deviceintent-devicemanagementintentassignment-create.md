---
title: Criar deviceManagementIntentAssignment
description: Criar um novo objeto deviceManagementIntentAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 573612fd318513b58da4c05351b8d785920811f5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313241"
---
# <a name="create-devicemanagementintentassignment"></a><span data-ttu-id="e0fcd-103">Criar deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="e0fcd-103">Create deviceManagementIntentAssignment</span></span>

> <span data-ttu-id="e0fcd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e0fcd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0fcd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0fcd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0fcd-106">Criar um novo objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e0fcd-106">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0fcd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e0fcd-107">Prerequisites</span></span>
<span data-ttu-id="e0fcd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0fcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0fcd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0fcd-110">Permission type</span></span>|<span data-ttu-id="e0fcd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e0fcd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0fcd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0fcd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0fcd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0fcd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0fcd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0fcd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0fcd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0fcd-115">Not supported.</span></span>|
|<span data-ttu-id="e0fcd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0fcd-116">Application</span></span>|<span data-ttu-id="e0fcd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0fcd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0fcd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0fcd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e0fcd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0fcd-119">Request headers</span></span>
|<span data-ttu-id="e0fcd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e0fcd-120">Header</span></span>|<span data-ttu-id="e0fcd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e0fcd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0fcd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0fcd-122">Authorization</span></span>|<span data-ttu-id="e0fcd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0fcd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0fcd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e0fcd-124">Accept</span></span>|<span data-ttu-id="e0fcd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0fcd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0fcd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0fcd-126">Request body</span></span>
<span data-ttu-id="e0fcd-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementIntentAssignment.</span><span class="sxs-lookup"><span data-stu-id="e0fcd-127">In the request body, supply a JSON representation for the deviceManagementIntentAssignment object.</span></span>

<span data-ttu-id="e0fcd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntentAssignment.</span><span class="sxs-lookup"><span data-stu-id="e0fcd-128">The following table shows the properties that are required when you create the deviceManagementIntentAssignment.</span></span>

|<span data-ttu-id="e0fcd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0fcd-129">Property</span></span>|<span data-ttu-id="e0fcd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0fcd-130">Type</span></span>|<span data-ttu-id="e0fcd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0fcd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0fcd-132">id</span><span class="sxs-lookup"><span data-stu-id="e0fcd-132">id</span></span>|<span data-ttu-id="e0fcd-133">String</span><span class="sxs-lookup"><span data-stu-id="e0fcd-133">String</span></span>|<span data-ttu-id="e0fcd-134">A ID da atribuição</span><span class="sxs-lookup"><span data-stu-id="e0fcd-134">The assignment ID</span></span>|
|<span data-ttu-id="e0fcd-135">destino</span><span class="sxs-lookup"><span data-stu-id="e0fcd-135">target</span></span>|[<span data-ttu-id="e0fcd-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e0fcd-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e0fcd-137">O destino da atribuição</span><span class="sxs-lookup"><span data-stu-id="e0fcd-137">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="e0fcd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0fcd-138">Response</span></span>
<span data-ttu-id="e0fcd-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0fcd-139">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0fcd-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0fcd-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0fcd-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0fcd-141">Request</span></span>
<span data-ttu-id="e0fcd-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0fcd-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e0fcd-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0fcd-143">Response</span></span>
<span data-ttu-id="e0fcd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0fcd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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







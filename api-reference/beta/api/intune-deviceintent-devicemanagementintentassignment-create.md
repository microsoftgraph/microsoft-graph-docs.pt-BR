---
title: Criar deviceManagementIntentAssignment
description: Criar um novo objeto deviceManagementIntentAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d3c6ea821bedb9489dc50a26808fa32086541774
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945834"
---
# <a name="create-devicemanagementintentassignment"></a><span data-ttu-id="7c4c3-103">Criar deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="7c4c3-103">Create deviceManagementIntentAssignment</span></span>

> <span data-ttu-id="7c4c3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c4c3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c4c3-106">Criar um novo objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="7c4c3-106">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c4c3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c4c3-107">Prerequisites</span></span>
<span data-ttu-id="7c4c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c4c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c4c3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c4c3-110">Permission type</span></span>|<span data-ttu-id="7c4c3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7c4c3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c4c3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c4c3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c4c3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c4c3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c4c3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c4c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c4c3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-115">Not supported.</span></span>|
|<span data-ttu-id="7c4c3-116">Application</span><span class="sxs-lookup"><span data-stu-id="7c4c3-116">Application</span></span>|<span data-ttu-id="7c4c3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c4c3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c4c3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c4c3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7c4c3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c4c3-119">Request headers</span></span>
|<span data-ttu-id="7c4c3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c4c3-120">Header</span></span>|<span data-ttu-id="7c4c3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7c4c3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c4c3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c4c3-122">Authorization</span></span>|<span data-ttu-id="7c4c3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c4c3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7c4c3-124">Accept</span></span>|<span data-ttu-id="7c4c3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c4c3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c4c3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c4c3-126">Request body</span></span>
<span data-ttu-id="7c4c3-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementIntentAssignment.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-127">In the request body, supply a JSON representation for the deviceManagementIntentAssignment object.</span></span>

<span data-ttu-id="7c4c3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntentAssignment.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-128">The following table shows the properties that are required when you create the deviceManagementIntentAssignment.</span></span>

|<span data-ttu-id="7c4c3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c4c3-129">Property</span></span>|<span data-ttu-id="7c4c3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c4c3-130">Type</span></span>|<span data-ttu-id="7c4c3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c4c3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c4c3-132">id</span><span class="sxs-lookup"><span data-stu-id="7c4c3-132">id</span></span>|<span data-ttu-id="7c4c3-133">String</span><span class="sxs-lookup"><span data-stu-id="7c4c3-133">String</span></span>|<span data-ttu-id="7c4c3-134">A ID da atribuição</span><span class="sxs-lookup"><span data-stu-id="7c4c3-134">The assignment ID</span></span>|
|<span data-ttu-id="7c4c3-135">destino</span><span class="sxs-lookup"><span data-stu-id="7c4c3-135">target</span></span>|[<span data-ttu-id="7c4c3-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7c4c3-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7c4c3-137">O destino da atribuição</span><span class="sxs-lookup"><span data-stu-id="7c4c3-137">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="7c4c3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c4c3-138">Response</span></span>
<span data-ttu-id="7c4c3-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-139">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c4c3-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c4c3-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c4c3-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c4c3-141">Request</span></span>
<span data-ttu-id="7c4c3-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c4c3-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c4c3-143">Response</span></span>
<span data-ttu-id="7c4c3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






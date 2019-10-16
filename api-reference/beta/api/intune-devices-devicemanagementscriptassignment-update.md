---
title: Atualizar deviceManagementScriptAssignment
description: Atualiza as propriedades de um objeto deviceManagementScriptAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e46fe73445f6af8f1e7e9ca44de4f6305ceb0eb7
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37530745"
---
# <a name="update-devicemanagementscriptassignment"></a><span data-ttu-id="8fc71-103">Atualizar deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="8fc71-103">Update deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="8fc71-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8fc71-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fc71-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8fc71-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fc71-106">Atualiza as propriedades de um objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8fc71-106">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fc71-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8fc71-107">Prerequisites</span></span>
<span data-ttu-id="8fc71-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fc71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fc71-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8fc71-110">Permission type</span></span>|<span data-ttu-id="8fc71-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8fc71-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fc71-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8fc71-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8fc71-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fc71-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8fc71-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8fc71-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fc71-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fc71-115">Not supported.</span></span>|
|<span data-ttu-id="8fc71-116">Application</span><span class="sxs-lookup"><span data-stu-id="8fc71-116">Application</span></span>|<span data-ttu-id="8fc71-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fc71-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fc71-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fc71-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceManagementScriptAssignmentId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="8fc71-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8fc71-119">Request headers</span></span>
|<span data-ttu-id="8fc71-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8fc71-120">Header</span></span>|<span data-ttu-id="8fc71-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8fc71-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fc71-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8fc71-122">Authorization</span></span>|<span data-ttu-id="8fc71-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8fc71-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fc71-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8fc71-124">Accept</span></span>|<span data-ttu-id="8fc71-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8fc71-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fc71-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8fc71-126">Request body</span></span>
<span data-ttu-id="8fc71-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8fc71-127">In the request body, supply a JSON representation for the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

<span data-ttu-id="8fc71-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8fc71-128">The following table shows the properties that are required when you create the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

|<span data-ttu-id="8fc71-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8fc71-129">Property</span></span>|<span data-ttu-id="8fc71-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8fc71-130">Type</span></span>|<span data-ttu-id="8fc71-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fc71-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fc71-132">id</span><span class="sxs-lookup"><span data-stu-id="8fc71-132">id</span></span>|<span data-ttu-id="8fc71-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8fc71-133">String</span></span>|<span data-ttu-id="8fc71-134">Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8fc71-134">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="8fc71-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8fc71-135">This property is read-only.</span></span>|
|<span data-ttu-id="8fc71-136">destino</span><span class="sxs-lookup"><span data-stu-id="8fc71-136">target</span></span>|[<span data-ttu-id="8fc71-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8fc71-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8fc71-138">A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.</span><span class="sxs-lookup"><span data-stu-id="8fc71-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="8fc71-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fc71-139">Response</span></span>
<span data-ttu-id="8fc71-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8fc71-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fc71-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8fc71-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fc71-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8fc71-142">Request</span></span>
<span data-ttu-id="8fc71-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8fc71-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceManagementScriptAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="8fc71-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fc71-144">Response</span></span>
<span data-ttu-id="8fc71-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8fc71-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```







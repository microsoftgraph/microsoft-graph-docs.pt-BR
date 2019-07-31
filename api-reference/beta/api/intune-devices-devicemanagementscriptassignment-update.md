---
title: Atualizar deviceManagementScriptAssignment
description: Atualiza as propriedades de um objeto deviceManagementScriptAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5a404e270e75dc08db88c444dd1967cc122efdc9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35986033"
---
# <a name="update-devicemanagementscriptassignment"></a><span data-ttu-id="6b102-103">Atualizar deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="6b102-103">Update deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="6b102-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b102-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b102-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b102-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b102-106">Atualiza as propriedades de um objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6b102-106">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b102-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6b102-107">Prerequisites</span></span>
<span data-ttu-id="6b102-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b102-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b102-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b102-110">Permission type</span></span>|<span data-ttu-id="6b102-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6b102-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b102-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b102-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b102-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b102-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6b102-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b102-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b102-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b102-115">Not supported.</span></span>|
|<span data-ttu-id="6b102-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b102-116">Application</span></span>|<span data-ttu-id="6b102-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b102-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b102-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b102-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6b102-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b102-119">Request headers</span></span>
|<span data-ttu-id="6b102-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b102-120">Header</span></span>|<span data-ttu-id="6b102-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6b102-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b102-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b102-122">Authorization</span></span>|<span data-ttu-id="6b102-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b102-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b102-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6b102-124">Accept</span></span>|<span data-ttu-id="6b102-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b102-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b102-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b102-126">Request body</span></span>
<span data-ttu-id="6b102-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6b102-127">In the request body, supply a JSON representation for the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

<span data-ttu-id="6b102-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6b102-128">The following table shows the properties that are required when you create the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

|<span data-ttu-id="6b102-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b102-129">Property</span></span>|<span data-ttu-id="6b102-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b102-130">Type</span></span>|<span data-ttu-id="6b102-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b102-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b102-132">id</span><span class="sxs-lookup"><span data-stu-id="6b102-132">id</span></span>|<span data-ttu-id="6b102-133">String</span><span class="sxs-lookup"><span data-stu-id="6b102-133">String</span></span>|<span data-ttu-id="6b102-134">Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6b102-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="6b102-135">destino</span><span class="sxs-lookup"><span data-stu-id="6b102-135">target</span></span>|[<span data-ttu-id="6b102-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6b102-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6b102-137">A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.</span><span class="sxs-lookup"><span data-stu-id="6b102-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="6b102-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b102-138">Response</span></span>
<span data-ttu-id="6b102-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b102-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b102-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b102-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b102-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b102-141">Request</span></span>
<span data-ttu-id="6b102-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b102-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="6b102-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b102-143">Response</span></span>
<span data-ttu-id="6b102-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b102-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






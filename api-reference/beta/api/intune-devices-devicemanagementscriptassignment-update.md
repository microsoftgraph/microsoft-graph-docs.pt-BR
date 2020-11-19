---
title: Atualizar deviceManagementScriptAssignment
description: Atualiza as propriedades de um objeto deviceManagementScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0210635d84b3d372ada520ec0440fa2df24d79cb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49263957"
---
# <a name="update-devicemanagementscriptassignment"></a><span data-ttu-id="b2e7a-103">Atualizar deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="b2e7a-103">Update deviceManagementScriptAssignment</span></span>

<span data-ttu-id="b2e7a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2e7a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2e7a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2e7a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2e7a-107">Atualiza as propriedades de um objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b2e7a-107">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2e7a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2e7a-108">Prerequisites</span></span>
<span data-ttu-id="b2e7a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2e7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2e7a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2e7a-111">Permission type</span></span>|<span data-ttu-id="b2e7a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2e7a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2e7a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2e7a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2e7a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2e7a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b2e7a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2e7a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2e7a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-116">Not supported.</span></span>|
|<span data-ttu-id="b2e7a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2e7a-117">Application</span></span>|<span data-ttu-id="b2e7a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2e7a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2e7a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2e7a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b2e7a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2e7a-120">Request headers</span></span>
|<span data-ttu-id="b2e7a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2e7a-121">Header</span></span>|<span data-ttu-id="b2e7a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b2e7a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2e7a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2e7a-123">Authorization</span></span>|<span data-ttu-id="b2e7a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2e7a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2e7a-125">Accept</span></span>|<span data-ttu-id="b2e7a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2e7a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2e7a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2e7a-127">Request body</span></span>
<span data-ttu-id="b2e7a-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b2e7a-128">In the request body, supply a JSON representation for the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

<span data-ttu-id="b2e7a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b2e7a-129">The following table shows the properties that are required when you create the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

|<span data-ttu-id="b2e7a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2e7a-130">Property</span></span>|<span data-ttu-id="b2e7a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2e7a-131">Type</span></span>|<span data-ttu-id="b2e7a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2e7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2e7a-133">id</span><span class="sxs-lookup"><span data-stu-id="b2e7a-133">id</span></span>|<span data-ttu-id="b2e7a-134">String</span><span class="sxs-lookup"><span data-stu-id="b2e7a-134">String</span></span>|<span data-ttu-id="b2e7a-135">Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="b2e7a-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-136">This property is read-only.</span></span>|
|<span data-ttu-id="b2e7a-137">destino</span><span class="sxs-lookup"><span data-stu-id="b2e7a-137">target</span></span>|[<span data-ttu-id="b2e7a-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b2e7a-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b2e7a-139">A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="b2e7a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2e7a-140">Response</span></span>
<span data-ttu-id="b2e7a-141">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2e7a-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2e7a-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2e7a-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2e7a-143">Request</span></span>
<span data-ttu-id="b2e7a-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
Content-type: application/json
Content-length: 327

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="b2e7a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2e7a-145">Response</span></span>
<span data-ttu-id="b2e7a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```





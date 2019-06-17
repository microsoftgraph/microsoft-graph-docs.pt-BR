---
title: Atualizar deviceManagementScriptAssignment
description: Atualiza as propriedades de um objeto deviceManagementScriptAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69e65b7b3265c3dade369b3f5cd5220ff378a6ff
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958967"
---
# <a name="update-devicemanagementscriptassignment"></a><span data-ttu-id="9285c-103">Atualizar deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="9285c-103">Update deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="9285c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9285c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9285c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9285c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9285c-106">Atualiza as propriedades de um objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9285c-106">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9285c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9285c-107">Prerequisites</span></span>
<span data-ttu-id="9285c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9285c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9285c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9285c-110">Permission type</span></span>|<span data-ttu-id="9285c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9285c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9285c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9285c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9285c-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9285c-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9285c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9285c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9285c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9285c-115">Not supported.</span></span>|
|<span data-ttu-id="9285c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9285c-116">Application</span></span>|<span data-ttu-id="9285c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9285c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9285c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9285c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9285c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9285c-119">Request headers</span></span>
|<span data-ttu-id="9285c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9285c-120">Header</span></span>|<span data-ttu-id="9285c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9285c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9285c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9285c-122">Authorization</span></span>|<span data-ttu-id="9285c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9285c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9285c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9285c-124">Accept</span></span>|<span data-ttu-id="9285c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9285c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9285c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9285c-126">Request body</span></span>
<span data-ttu-id="9285c-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9285c-127">In the request body, supply a JSON representation for the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

<span data-ttu-id="9285c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9285c-128">The following table shows the properties that are required when you create the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

|<span data-ttu-id="9285c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9285c-129">Property</span></span>|<span data-ttu-id="9285c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9285c-130">Type</span></span>|<span data-ttu-id="9285c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9285c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9285c-132">id</span><span class="sxs-lookup"><span data-stu-id="9285c-132">id</span></span>|<span data-ttu-id="9285c-133">String</span><span class="sxs-lookup"><span data-stu-id="9285c-133">String</span></span>|<span data-ttu-id="9285c-134">Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9285c-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="9285c-135">destino</span><span class="sxs-lookup"><span data-stu-id="9285c-135">target</span></span>|[<span data-ttu-id="9285c-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9285c-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9285c-137">A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.</span><span class="sxs-lookup"><span data-stu-id="9285c-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="9285c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9285c-138">Response</span></span>
<span data-ttu-id="9285c-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9285c-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9285c-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9285c-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="9285c-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9285c-141">Request</span></span>
<span data-ttu-id="9285c-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9285c-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9285c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9285c-143">Response</span></span>
<span data-ttu-id="9285c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9285c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






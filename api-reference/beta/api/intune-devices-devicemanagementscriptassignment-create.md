---
title: Criar deviceManagementScriptAssignment
description: Criar um novo objeto deviceManagementScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d809117c8503ef625b88e19d912a3360a947a06
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076943"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="40196-103">Criar deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="40196-103">Create deviceManagementScriptAssignment</span></span>

<span data-ttu-id="40196-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40196-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40196-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40196-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40196-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40196-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40196-107">Criar um novo objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="40196-107">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40196-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40196-108">Prerequisites</span></span>
<span data-ttu-id="40196-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40196-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40196-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40196-111">Permission type</span></span>|<span data-ttu-id="40196-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="40196-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40196-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40196-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40196-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40196-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="40196-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40196-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40196-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40196-116">Not supported.</span></span>|
|<span data-ttu-id="40196-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40196-117">Application</span></span>|<span data-ttu-id="40196-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40196-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40196-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40196-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="40196-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40196-120">Request headers</span></span>
|<span data-ttu-id="40196-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40196-121">Header</span></span>|<span data-ttu-id="40196-122">Valor</span><span class="sxs-lookup"><span data-stu-id="40196-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40196-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="40196-123">Authorization</span></span>|<span data-ttu-id="40196-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40196-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40196-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="40196-125">Accept</span></span>|<span data-ttu-id="40196-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40196-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40196-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40196-127">Request body</span></span>
<span data-ttu-id="40196-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="40196-128">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="40196-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="40196-129">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="40196-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40196-130">Property</span></span>|<span data-ttu-id="40196-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="40196-131">Type</span></span>|<span data-ttu-id="40196-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="40196-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40196-133">id</span><span class="sxs-lookup"><span data-stu-id="40196-133">id</span></span>|<span data-ttu-id="40196-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40196-134">String</span></span>|<span data-ttu-id="40196-135">Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="40196-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="40196-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40196-136">This property is read-only.</span></span>|
|<span data-ttu-id="40196-137">destino</span><span class="sxs-lookup"><span data-stu-id="40196-137">target</span></span>|[<span data-ttu-id="40196-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="40196-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="40196-139">A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.</span><span class="sxs-lookup"><span data-stu-id="40196-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="40196-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="40196-140">Response</span></span>
<span data-ttu-id="40196-141">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40196-141">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40196-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40196-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="40196-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40196-143">Request</span></span>
<span data-ttu-id="40196-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40196-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
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

### <a name="response"></a><span data-ttu-id="40196-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="40196-145">Response</span></span>
<span data-ttu-id="40196-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40196-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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







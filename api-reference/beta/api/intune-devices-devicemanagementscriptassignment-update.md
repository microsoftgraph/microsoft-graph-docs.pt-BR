---
title: Atualizar deviceManagementScriptAssignment
description: Atualizar as propriedades de um objeto deviceManagementScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 42c1f2111afaf8482635228e7c4310dbc8f88b2e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156424"
---
# <a name="update-devicemanagementscriptassignment"></a><span data-ttu-id="8af13-103">Atualizar deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="8af13-103">Update deviceManagementScriptAssignment</span></span>

<span data-ttu-id="8af13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8af13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8af13-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8af13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8af13-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8af13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8af13-107">Atualizar as propriedades de um [objeto deviceManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8af13-107">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8af13-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8af13-108">Prerequisites</span></span>
<span data-ttu-id="8af13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8af13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8af13-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8af13-111">Permission type</span></span>|<span data-ttu-id="8af13-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8af13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8af13-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8af13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8af13-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8af13-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8af13-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8af13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8af13-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8af13-116">Not supported.</span></span>|
|<span data-ttu-id="8af13-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8af13-117">Application</span></span>|<span data-ttu-id="8af13-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8af13-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8af13-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8af13-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="8af13-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8af13-120">Request headers</span></span>
|<span data-ttu-id="8af13-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8af13-121">Header</span></span>|<span data-ttu-id="8af13-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8af13-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8af13-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8af13-123">Authorization</span></span>|<span data-ttu-id="8af13-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8af13-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8af13-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8af13-125">Accept</span></span>|<span data-ttu-id="8af13-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8af13-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8af13-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8af13-127">Request body</span></span>
<span data-ttu-id="8af13-128">No corpo da solicitação, fornece uma representação JSON do [objeto deviceManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8af13-128">In the request body, supply a JSON representation for the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

<span data-ttu-id="8af13-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8af13-129">The following table shows the properties that are required when you create the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

|<span data-ttu-id="8af13-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8af13-130">Property</span></span>|<span data-ttu-id="8af13-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8af13-131">Type</span></span>|<span data-ttu-id="8af13-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8af13-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8af13-133">id</span><span class="sxs-lookup"><span data-stu-id="8af13-133">id</span></span>|<span data-ttu-id="8af13-134">String</span><span class="sxs-lookup"><span data-stu-id="8af13-134">String</span></span>|<span data-ttu-id="8af13-135">Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8af13-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="8af13-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8af13-136">This property is read-only.</span></span>|
|<span data-ttu-id="8af13-137">destino</span><span class="sxs-lookup"><span data-stu-id="8af13-137">target</span></span>|[<span data-ttu-id="8af13-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8af13-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8af13-139">A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.</span><span class="sxs-lookup"><span data-stu-id="8af13-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="8af13-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8af13-140">Response</span></span>
<span data-ttu-id="8af13-141">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8af13-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8af13-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8af13-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="8af13-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8af13-143">Request</span></span>
<span data-ttu-id="8af13-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8af13-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="8af13-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8af13-145">Response</span></span>
<span data-ttu-id="8af13-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8af13-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```





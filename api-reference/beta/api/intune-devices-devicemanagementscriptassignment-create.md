---
title: Criar deviceManagementScriptAssignment
description: Crie um novo objeto deviceManagementScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9fbb39816cc4a542c74fd166be431df2e71f7273
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611990"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="a3eca-103">Criar deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="a3eca-103">Create deviceManagementScriptAssignment</span></span>

<span data-ttu-id="a3eca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3eca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3eca-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a3eca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3eca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a3eca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3eca-107">Crie um novo [objeto deviceManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a3eca-107">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3eca-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a3eca-108">Prerequisites</span></span>
<span data-ttu-id="a3eca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3eca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3eca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3eca-111">Permission type</span></span>|<span data-ttu-id="a3eca-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3eca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3eca-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3eca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3eca-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3eca-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a3eca-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3eca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3eca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3eca-116">Not supported.</span></span>|
|<span data-ttu-id="a3eca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3eca-117">Application</span></span>|<span data-ttu-id="a3eca-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3eca-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3eca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3eca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
POST /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a3eca-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3eca-120">Request headers</span></span>
|<span data-ttu-id="a3eca-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3eca-121">Header</span></span>|<span data-ttu-id="a3eca-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a3eca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3eca-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3eca-123">Authorization</span></span>|<span data-ttu-id="a3eca-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3eca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3eca-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a3eca-125">Accept</span></span>|<span data-ttu-id="a3eca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3eca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3eca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3eca-127">Request body</span></span>
<span data-ttu-id="a3eca-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="a3eca-128">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="a3eca-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="a3eca-129">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="a3eca-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3eca-130">Property</span></span>|<span data-ttu-id="a3eca-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3eca-131">Type</span></span>|<span data-ttu-id="a3eca-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3eca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3eca-133">id</span><span class="sxs-lookup"><span data-stu-id="a3eca-133">id</span></span>|<span data-ttu-id="a3eca-134">String</span><span class="sxs-lookup"><span data-stu-id="a3eca-134">String</span></span>|<span data-ttu-id="a3eca-135">Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a3eca-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="a3eca-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a3eca-136">This property is read-only.</span></span>|
|<span data-ttu-id="a3eca-137">destino</span><span class="sxs-lookup"><span data-stu-id="a3eca-137">target</span></span>|[<span data-ttu-id="a3eca-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a3eca-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a3eca-139">A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.</span><span class="sxs-lookup"><span data-stu-id="a3eca-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="a3eca-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3eca-140">Response</span></span>
<span data-ttu-id="a3eca-141">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3eca-141">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3eca-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3eca-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3eca-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3eca-143">Request</span></span>
<span data-ttu-id="a3eca-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3eca-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
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

### <a name="response"></a><span data-ttu-id="a3eca-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3eca-145">Response</span></span>
<span data-ttu-id="a3eca-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3eca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





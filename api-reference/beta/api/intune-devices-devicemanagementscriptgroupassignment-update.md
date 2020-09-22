---
title: Atualizar deviceManagementScriptGroupAssignment
description: Atualiza as propriedades de um objeto deviceManagementScriptGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8cc11537c586f55eb99c27ca6abc43255f80b4da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48014571"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="8e800-103">Atualizar deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="8e800-103">Update deviceManagementScriptGroupAssignment</span></span>

<span data-ttu-id="8e800-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8e800-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e800-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e800-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e800-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e800-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e800-107">Atualiza as propriedades de um objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8e800-107">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e800-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e800-108">Prerequisites</span></span>
<span data-ttu-id="8e800-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e800-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e800-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e800-111">Permission type</span></span>|<span data-ttu-id="8e800-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8e800-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e800-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e800-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e800-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e800-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8e800-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e800-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e800-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e800-116">Not supported.</span></span>|
|<span data-ttu-id="8e800-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e800-117">Application</span></span>|<span data-ttu-id="8e800-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e800-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e800-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e800-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="8e800-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e800-120">Request headers</span></span>
|<span data-ttu-id="8e800-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e800-121">Header</span></span>|<span data-ttu-id="8e800-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8e800-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e800-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e800-123">Authorization</span></span>|<span data-ttu-id="8e800-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e800-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e800-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e800-125">Accept</span></span>|<span data-ttu-id="8e800-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e800-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e800-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e800-127">Request body</span></span>
<span data-ttu-id="8e800-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8e800-128">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="8e800-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8e800-129">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="8e800-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e800-130">Property</span></span>|<span data-ttu-id="8e800-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e800-131">Type</span></span>|<span data-ttu-id="8e800-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e800-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e800-133">id</span><span class="sxs-lookup"><span data-stu-id="8e800-133">id</span></span>|<span data-ttu-id="8e800-134">String</span><span class="sxs-lookup"><span data-stu-id="8e800-134">String</span></span>|<span data-ttu-id="8e800-135">Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8e800-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="8e800-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e800-136">This property is read-only.</span></span>|
|<span data-ttu-id="8e800-137">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="8e800-137">targetGroupId</span></span>|<span data-ttu-id="8e800-138">String</span><span class="sxs-lookup"><span data-stu-id="8e800-138">String</span></span>|<span data-ttu-id="8e800-139">A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.</span><span class="sxs-lookup"><span data-stu-id="8e800-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="8e800-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e800-140">Response</span></span>
<span data-ttu-id="8e800-141">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e800-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e800-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e800-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e800-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e800-143">Request</span></span>
<span data-ttu-id="8e800-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e800-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="8e800-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e800-145">Response</span></span>
<span data-ttu-id="8e800-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e800-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```







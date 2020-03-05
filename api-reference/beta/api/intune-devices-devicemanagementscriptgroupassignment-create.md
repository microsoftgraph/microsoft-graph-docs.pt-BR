---
title: Criar deviceManagementScriptGroupAssignment
description: Criar um novo objeto deviceManagementScriptGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6542170b28dc326d4bf96616cc982395244dd5ca
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469360"
---
# <a name="create-devicemanagementscriptgroupassignment"></a><span data-ttu-id="0fc21-103">Criar deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="0fc21-103">Create deviceManagementScriptGroupAssignment</span></span>

<span data-ttu-id="0fc21-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0fc21-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fc21-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0fc21-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fc21-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0fc21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fc21-107">Criar um novo objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="0fc21-107">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fc21-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0fc21-108">Prerequisites</span></span>
<span data-ttu-id="0fc21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fc21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fc21-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fc21-111">Permission type</span></span>|<span data-ttu-id="0fc21-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0fc21-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fc21-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fc21-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0fc21-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fc21-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0fc21-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fc21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fc21-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fc21-116">Not supported.</span></span>|
|<span data-ttu-id="0fc21-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fc21-117">Application</span></span>|<span data-ttu-id="0fc21-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fc21-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fc21-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fc21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="0fc21-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fc21-120">Request headers</span></span>
|<span data-ttu-id="0fc21-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0fc21-121">Header</span></span>|<span data-ttu-id="0fc21-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0fc21-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fc21-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fc21-123">Authorization</span></span>|<span data-ttu-id="0fc21-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fc21-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fc21-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0fc21-125">Accept</span></span>|<span data-ttu-id="0fc21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0fc21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fc21-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fc21-127">Request body</span></span>
<span data-ttu-id="0fc21-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScriptGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="0fc21-128">In the request body, supply a JSON representation for the deviceManagementScriptGroupAssignment object.</span></span>

<span data-ttu-id="0fc21-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScriptGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="0fc21-129">The following table shows the properties that are required when you create the deviceManagementScriptGroupAssignment.</span></span>

|<span data-ttu-id="0fc21-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0fc21-130">Property</span></span>|<span data-ttu-id="0fc21-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0fc21-131">Type</span></span>|<span data-ttu-id="0fc21-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fc21-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fc21-133">id</span><span class="sxs-lookup"><span data-stu-id="0fc21-133">id</span></span>|<span data-ttu-id="0fc21-134">String</span><span class="sxs-lookup"><span data-stu-id="0fc21-134">String</span></span>|<span data-ttu-id="0fc21-135">Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0fc21-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="0fc21-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0fc21-136">This property is read-only.</span></span>|
|<span data-ttu-id="0fc21-137">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="0fc21-137">targetGroupId</span></span>|<span data-ttu-id="0fc21-138">String</span><span class="sxs-lookup"><span data-stu-id="0fc21-138">String</span></span>|<span data-ttu-id="0fc21-139">A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.</span><span class="sxs-lookup"><span data-stu-id="0fc21-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="0fc21-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fc21-140">Response</span></span>
<span data-ttu-id="0fc21-141">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fc21-141">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fc21-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fc21-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fc21-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fc21-143">Request</span></span>
<span data-ttu-id="0fc21-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fc21-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="0fc21-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fc21-145">Response</span></span>
<span data-ttu-id="0fc21-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fc21-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```






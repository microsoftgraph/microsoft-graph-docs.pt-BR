---
title: Criar deviceManagementScriptGroupAssignment
description: Criar um novo objeto deviceManagementScriptGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f3cb20edd465ea9af0efe9a3e0a8ce457b7ad44
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37180500"
---
# <a name="create-devicemanagementscriptgroupassignment"></a><span data-ttu-id="53451-103">Criar deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="53451-103">Create deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="53451-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="53451-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53451-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53451-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53451-106">Criar um novo objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="53451-106">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53451-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53451-107">Prerequisites</span></span>
<span data-ttu-id="53451-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53451-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53451-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53451-110">Permission type</span></span>|<span data-ttu-id="53451-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="53451-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53451-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53451-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53451-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53451-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="53451-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53451-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53451-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53451-115">Not supported.</span></span>|
|<span data-ttu-id="53451-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53451-116">Application</span></span>|<span data-ttu-id="53451-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53451-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53451-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53451-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="53451-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53451-119">Request headers</span></span>
|<span data-ttu-id="53451-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53451-120">Header</span></span>|<span data-ttu-id="53451-121">Valor</span><span class="sxs-lookup"><span data-stu-id="53451-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53451-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="53451-122">Authorization</span></span>|<span data-ttu-id="53451-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53451-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53451-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="53451-124">Accept</span></span>|<span data-ttu-id="53451-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53451-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53451-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53451-126">Request body</span></span>
<span data-ttu-id="53451-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScriptGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="53451-127">In the request body, supply a JSON representation for the deviceManagementScriptGroupAssignment object.</span></span>

<span data-ttu-id="53451-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScriptGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="53451-128">The following table shows the properties that are required when you create the deviceManagementScriptGroupAssignment.</span></span>

|<span data-ttu-id="53451-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53451-129">Property</span></span>|<span data-ttu-id="53451-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="53451-130">Type</span></span>|<span data-ttu-id="53451-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="53451-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53451-132">id</span><span class="sxs-lookup"><span data-stu-id="53451-132">id</span></span>|<span data-ttu-id="53451-133">String</span><span class="sxs-lookup"><span data-stu-id="53451-133">String</span></span>|<span data-ttu-id="53451-134">Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="53451-134">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="53451-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53451-135">This property is read-only.</span></span>|
|<span data-ttu-id="53451-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="53451-136">targetGroupId</span></span>|<span data-ttu-id="53451-137">String</span><span class="sxs-lookup"><span data-stu-id="53451-137">String</span></span>|<span data-ttu-id="53451-138">A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.</span><span class="sxs-lookup"><span data-stu-id="53451-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="53451-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="53451-139">Response</span></span>
<span data-ttu-id="53451-140">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53451-140">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53451-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53451-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="53451-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53451-142">Request</span></span>
<span data-ttu-id="53451-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53451-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="53451-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="53451-144">Response</span></span>
<span data-ttu-id="53451-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53451-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





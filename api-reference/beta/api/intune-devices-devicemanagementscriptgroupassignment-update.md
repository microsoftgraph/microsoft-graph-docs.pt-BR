---
title: Atualizar deviceManagementScriptGroupAssignment
description: Atualiza as propriedades de um objeto deviceManagementScriptGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 542967403d7e1a18576b8c665c1121be2b3c8f0a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958806"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="bddef-103">Atualizar deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="bddef-103">Update deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="bddef-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bddef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bddef-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bddef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bddef-106">Atualiza as propriedades de um objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="bddef-106">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bddef-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bddef-107">Prerequisites</span></span>
<span data-ttu-id="bddef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bddef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bddef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bddef-110">Permission type</span></span>|<span data-ttu-id="bddef-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bddef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bddef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bddef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bddef-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bddef-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bddef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bddef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bddef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bddef-115">Not supported.</span></span>|
|<span data-ttu-id="bddef-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bddef-116">Application</span></span>|<span data-ttu-id="bddef-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bddef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bddef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bddef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="bddef-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bddef-119">Request headers</span></span>
|<span data-ttu-id="bddef-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bddef-120">Header</span></span>|<span data-ttu-id="bddef-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bddef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bddef-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bddef-122">Authorization</span></span>|<span data-ttu-id="bddef-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bddef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bddef-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bddef-124">Accept</span></span>|<span data-ttu-id="bddef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bddef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bddef-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bddef-126">Request body</span></span>
<span data-ttu-id="bddef-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="bddef-127">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="bddef-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bddef-128">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="bddef-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bddef-129">Property</span></span>|<span data-ttu-id="bddef-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bddef-130">Type</span></span>|<span data-ttu-id="bddef-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bddef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bddef-132">id</span><span class="sxs-lookup"><span data-stu-id="bddef-132">id</span></span>|<span data-ttu-id="bddef-133">String</span><span class="sxs-lookup"><span data-stu-id="bddef-133">String</span></span>|<span data-ttu-id="bddef-134">Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="bddef-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="bddef-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="bddef-135">targetGroupId</span></span>|<span data-ttu-id="bddef-136">String</span><span class="sxs-lookup"><span data-stu-id="bddef-136">String</span></span>|<span data-ttu-id="bddef-137">A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.</span><span class="sxs-lookup"><span data-stu-id="bddef-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="bddef-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="bddef-138">Response</span></span>
<span data-ttu-id="bddef-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bddef-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bddef-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bddef-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="bddef-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bddef-141">Request</span></span>
<span data-ttu-id="bddef-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bddef-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="bddef-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="bddef-143">Response</span></span>
<span data-ttu-id="bddef-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bddef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






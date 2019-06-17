---
title: Criar deviceManagementScriptAssignment
description: Criar um novo objeto deviceManagementScriptAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 898a70dbabcbff69edb4e2287dfa7ed29d24ddd2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959023"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="d392e-103">Criar deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d392e-103">Create deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="d392e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d392e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d392e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d392e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d392e-106">Criar um novo objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d392e-106">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d392e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d392e-107">Prerequisites</span></span>
<span data-ttu-id="d392e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d392e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d392e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d392e-110">Permission type</span></span>|<span data-ttu-id="d392e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d392e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d392e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d392e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d392e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d392e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d392e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d392e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d392e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d392e-115">Not supported.</span></span>|
|<span data-ttu-id="d392e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d392e-116">Application</span></span>|<span data-ttu-id="d392e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d392e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d392e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d392e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d392e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d392e-119">Request headers</span></span>
|<span data-ttu-id="d392e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d392e-120">Header</span></span>|<span data-ttu-id="d392e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d392e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d392e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d392e-122">Authorization</span></span>|<span data-ttu-id="d392e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d392e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d392e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d392e-124">Accept</span></span>|<span data-ttu-id="d392e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d392e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d392e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d392e-126">Request body</span></span>
<span data-ttu-id="d392e-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="d392e-127">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="d392e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="d392e-128">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="d392e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d392e-129">Property</span></span>|<span data-ttu-id="d392e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d392e-130">Type</span></span>|<span data-ttu-id="d392e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d392e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d392e-132">id</span><span class="sxs-lookup"><span data-stu-id="d392e-132">id</span></span>|<span data-ttu-id="d392e-133">String</span><span class="sxs-lookup"><span data-stu-id="d392e-133">String</span></span>|<span data-ttu-id="d392e-134">Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d392e-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="d392e-135">destino</span><span class="sxs-lookup"><span data-stu-id="d392e-135">target</span></span>|[<span data-ttu-id="d392e-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d392e-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d392e-137">A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.</span><span class="sxs-lookup"><span data-stu-id="d392e-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="d392e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d392e-138">Response</span></span>
<span data-ttu-id="d392e-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d392e-139">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d392e-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d392e-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="d392e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d392e-141">Request</span></span>
<span data-ttu-id="d392e-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d392e-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d392e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d392e-143">Response</span></span>
<span data-ttu-id="d392e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d392e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






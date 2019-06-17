---
title: Criar deviceManagementScriptGroupAssignment
description: Criar um novo objeto deviceManagementScriptGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e3079da0aadd24ef0b36d3e5a02c9c979380c37
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958883"
---
# <a name="create-devicemanagementscriptgroupassignment"></a><span data-ttu-id="0be87-103">Criar deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="0be87-103">Create deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="0be87-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0be87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0be87-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0be87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0be87-106">Criar um novo objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="0be87-106">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0be87-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0be87-107">Prerequisites</span></span>
<span data-ttu-id="0be87-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0be87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0be87-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0be87-110">Permission type</span></span>|<span data-ttu-id="0be87-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0be87-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0be87-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0be87-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0be87-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be87-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0be87-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0be87-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0be87-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0be87-115">Not supported.</span></span>|
|<span data-ttu-id="0be87-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0be87-116">Application</span></span>|<span data-ttu-id="0be87-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0be87-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0be87-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0be87-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="0be87-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0be87-119">Request headers</span></span>
|<span data-ttu-id="0be87-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0be87-120">Header</span></span>|<span data-ttu-id="0be87-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0be87-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0be87-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0be87-122">Authorization</span></span>|<span data-ttu-id="0be87-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0be87-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0be87-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0be87-124">Accept</span></span>|<span data-ttu-id="0be87-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0be87-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0be87-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0be87-126">Request body</span></span>
<span data-ttu-id="0be87-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScriptGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="0be87-127">In the request body, supply a JSON representation for the deviceManagementScriptGroupAssignment object.</span></span>

<span data-ttu-id="0be87-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScriptGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="0be87-128">The following table shows the properties that are required when you create the deviceManagementScriptGroupAssignment.</span></span>

|<span data-ttu-id="0be87-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0be87-129">Property</span></span>|<span data-ttu-id="0be87-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0be87-130">Type</span></span>|<span data-ttu-id="0be87-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0be87-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0be87-132">id</span><span class="sxs-lookup"><span data-stu-id="0be87-132">id</span></span>|<span data-ttu-id="0be87-133">String</span><span class="sxs-lookup"><span data-stu-id="0be87-133">String</span></span>|<span data-ttu-id="0be87-134">Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0be87-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="0be87-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="0be87-135">targetGroupId</span></span>|<span data-ttu-id="0be87-136">String</span><span class="sxs-lookup"><span data-stu-id="0be87-136">String</span></span>|<span data-ttu-id="0be87-137">A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.</span><span class="sxs-lookup"><span data-stu-id="0be87-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="0be87-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0be87-138">Response</span></span>
<span data-ttu-id="0be87-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0be87-139">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0be87-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0be87-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="0be87-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0be87-141">Request</span></span>
<span data-ttu-id="0be87-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0be87-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="0be87-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="0be87-143">Response</span></span>
<span data-ttu-id="0be87-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0be87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






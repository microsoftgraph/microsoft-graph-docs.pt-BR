---
title: Criar deviceManagementScriptGroupAssignment
description: Criar um novo objeto deviceManagementScriptGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9f5f5d1235750a2c27f871c7f1c10295ba426331
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47974370"
---
# <a name="create-devicemanagementscriptgroupassignment"></a><span data-ttu-id="b0885-103">Criar deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="b0885-103">Create deviceManagementScriptGroupAssignment</span></span>

<span data-ttu-id="b0885-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0885-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0885-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0885-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0885-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0885-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0885-107">Criar um novo objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b0885-107">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0885-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0885-108">Prerequisites</span></span>
<span data-ttu-id="b0885-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0885-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0885-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0885-111">Permission type</span></span>|<span data-ttu-id="b0885-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0885-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0885-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0885-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0885-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0885-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b0885-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0885-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0885-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0885-116">Not supported.</span></span>|
|<span data-ttu-id="b0885-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0885-117">Application</span></span>|<span data-ttu-id="b0885-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0885-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0885-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0885-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="b0885-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0885-120">Request headers</span></span>
|<span data-ttu-id="b0885-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0885-121">Header</span></span>|<span data-ttu-id="b0885-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b0885-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0885-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0885-123">Authorization</span></span>|<span data-ttu-id="b0885-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0885-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0885-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b0885-125">Accept</span></span>|<span data-ttu-id="b0885-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0885-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0885-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0885-127">Request body</span></span>
<span data-ttu-id="b0885-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScriptGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="b0885-128">In the request body, supply a JSON representation for the deviceManagementScriptGroupAssignment object.</span></span>

<span data-ttu-id="b0885-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScriptGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="b0885-129">The following table shows the properties that are required when you create the deviceManagementScriptGroupAssignment.</span></span>

|<span data-ttu-id="b0885-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0885-130">Property</span></span>|<span data-ttu-id="b0885-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0885-131">Type</span></span>|<span data-ttu-id="b0885-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0885-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0885-133">id</span><span class="sxs-lookup"><span data-stu-id="b0885-133">id</span></span>|<span data-ttu-id="b0885-134">String</span><span class="sxs-lookup"><span data-stu-id="b0885-134">String</span></span>|<span data-ttu-id="b0885-135">Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b0885-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="b0885-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0885-136">This property is read-only.</span></span>|
|<span data-ttu-id="b0885-137">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="b0885-137">targetGroupId</span></span>|<span data-ttu-id="b0885-138">String</span><span class="sxs-lookup"><span data-stu-id="b0885-138">String</span></span>|<span data-ttu-id="b0885-139">A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.</span><span class="sxs-lookup"><span data-stu-id="b0885-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="b0885-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0885-140">Response</span></span>
<span data-ttu-id="b0885-141">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0885-141">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0885-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0885-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0885-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0885-143">Request</span></span>
<span data-ttu-id="b0885-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0885-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="b0885-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0885-145">Response</span></span>
<span data-ttu-id="b0885-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0885-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







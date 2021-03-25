---
title: Criar deviceManagementScriptGroupAssignment
description: Crie um novo objeto deviceManagementScriptGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff1384b470d723e083e7070c2892f164a9775020
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150451"
---
# <a name="create-devicemanagementscriptgroupassignment"></a><span data-ttu-id="0dd31-103">Criar deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="0dd31-103">Create deviceManagementScriptGroupAssignment</span></span>

<span data-ttu-id="0dd31-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dd31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0dd31-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0dd31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0dd31-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0dd31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dd31-107">Crie um novo [objeto deviceManagementScriptGroupAssignment.](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0dd31-107">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0dd31-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0dd31-108">Prerequisites</span></span>
<span data-ttu-id="0dd31-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0dd31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0dd31-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0dd31-111">Permission type</span></span>|<span data-ttu-id="0dd31-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0dd31-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0dd31-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0dd31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0dd31-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dd31-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0dd31-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0dd31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0dd31-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0dd31-116">Not supported.</span></span>|
|<span data-ttu-id="0dd31-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0dd31-117">Application</span></span>|<span data-ttu-id="0dd31-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dd31-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0dd31-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0dd31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
POST /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="0dd31-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0dd31-120">Request headers</span></span>
|<span data-ttu-id="0dd31-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0dd31-121">Header</span></span>|<span data-ttu-id="0dd31-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0dd31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0dd31-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0dd31-123">Authorization</span></span>|<span data-ttu-id="0dd31-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0dd31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0dd31-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0dd31-125">Accept</span></span>|<span data-ttu-id="0dd31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0dd31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0dd31-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0dd31-127">Request body</span></span>
<span data-ttu-id="0dd31-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementScriptGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="0dd31-128">In the request body, supply a JSON representation for the deviceManagementScriptGroupAssignment object.</span></span>

<span data-ttu-id="0dd31-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScriptGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="0dd31-129">The following table shows the properties that are required when you create the deviceManagementScriptGroupAssignment.</span></span>

|<span data-ttu-id="0dd31-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0dd31-130">Property</span></span>|<span data-ttu-id="0dd31-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0dd31-131">Type</span></span>|<span data-ttu-id="0dd31-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0dd31-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dd31-133">id</span><span class="sxs-lookup"><span data-stu-id="0dd31-133">id</span></span>|<span data-ttu-id="0dd31-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0dd31-134">String</span></span>|<span data-ttu-id="0dd31-135">Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0dd31-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="0dd31-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0dd31-136">This property is read-only.</span></span>|
|<span data-ttu-id="0dd31-137">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="0dd31-137">targetGroupId</span></span>|<span data-ttu-id="0dd31-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0dd31-138">String</span></span>|<span data-ttu-id="0dd31-139">A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.</span><span class="sxs-lookup"><span data-stu-id="0dd31-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="0dd31-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0dd31-140">Response</span></span>
<span data-ttu-id="0dd31-141">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0dd31-141">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0dd31-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0dd31-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="0dd31-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0dd31-143">Request</span></span>
<span data-ttu-id="0dd31-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0dd31-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="0dd31-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="0dd31-145">Response</span></span>
<span data-ttu-id="0dd31-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0dd31-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





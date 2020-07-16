---
title: Criar groupPolicyConfigurationAssignment
description: Criar um novo objeto groupPolicyConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b21781985c0ae6d48db1cb7a264989075bcfaa37
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791984"
---
# <a name="create-grouppolicyconfigurationassignment"></a><span data-ttu-id="cf66e-103">Criar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="cf66e-103">Create groupPolicyConfigurationAssignment</span></span>

<span data-ttu-id="cf66e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf66e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf66e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf66e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf66e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf66e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf66e-107">Criar um novo objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="cf66e-107">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf66e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf66e-108">Prerequisites</span></span>
<span data-ttu-id="cf66e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf66e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf66e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf66e-111">Permission type</span></span>|<span data-ttu-id="cf66e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf66e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf66e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf66e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf66e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf66e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf66e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf66e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf66e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf66e-116">Not supported.</span></span>|
|<span data-ttu-id="cf66e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf66e-117">Application</span></span>|<span data-ttu-id="cf66e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf66e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf66e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf66e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="cf66e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf66e-120">Request headers</span></span>
|<span data-ttu-id="cf66e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf66e-121">Header</span></span>|<span data-ttu-id="cf66e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cf66e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf66e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf66e-123">Authorization</span></span>|<span data-ttu-id="cf66e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf66e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf66e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf66e-125">Accept</span></span>|<span data-ttu-id="cf66e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf66e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf66e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf66e-127">Request body</span></span>
<span data-ttu-id="cf66e-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="cf66e-128">In the request body, supply a JSON representation for the groupPolicyConfigurationAssignment object.</span></span>

<span data-ttu-id="cf66e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="cf66e-129">The following table shows the properties that are required when you create the groupPolicyConfigurationAssignment.</span></span>

|<span data-ttu-id="cf66e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf66e-130">Property</span></span>|<span data-ttu-id="cf66e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf66e-131">Type</span></span>|<span data-ttu-id="cf66e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf66e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf66e-133">id</span><span class="sxs-lookup"><span data-stu-id="cf66e-133">id</span></span>|<span data-ttu-id="cf66e-134">String</span><span class="sxs-lookup"><span data-stu-id="cf66e-134">String</span></span>|<span data-ttu-id="cf66e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cf66e-135">Key of the entity.</span></span>|
|<span data-ttu-id="cf66e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf66e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cf66e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf66e-137">DateTimeOffset</span></span>|<span data-ttu-id="cf66e-138">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cf66e-138">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="cf66e-139">destino</span><span class="sxs-lookup"><span data-stu-id="cf66e-139">target</span></span>|[<span data-ttu-id="cf66e-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cf66e-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cf66e-141">O tipo de grupo de destino da configuração da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="cf66e-141">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="cf66e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf66e-142">Response</span></span>
<span data-ttu-id="cf66e-143">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf66e-143">If successful, this method returns a `201 Created` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf66e-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf66e-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf66e-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf66e-145">Request</span></span>
<span data-ttu-id="cf66e-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf66e-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
Content-type: application/json
Content-length: 329

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="cf66e-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf66e-147">Response</span></span>
<span data-ttu-id="cf66e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf66e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 442

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




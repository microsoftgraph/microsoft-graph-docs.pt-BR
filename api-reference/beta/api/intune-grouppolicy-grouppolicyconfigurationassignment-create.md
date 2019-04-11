---
title: Criar groupPolicyConfigurationAssignment
description: Criar um novo objeto groupPolicyConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b0deda8c76a52705a60787766711b18b4b6ff50
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780606"
---
# <a name="create-grouppolicyconfigurationassignment"></a><span data-ttu-id="cfdfd-103">Criar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="cfdfd-103">Create groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="cfdfd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cfdfd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfdfd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cfdfd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfdfd-106">Criar um novo objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="cfdfd-106">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cfdfd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cfdfd-107">Prerequisites</span></span>
<span data-ttu-id="cfdfd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfdfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfdfd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfdfd-110">Permission type</span></span>|<span data-ttu-id="cfdfd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cfdfd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfdfd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfdfd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cfdfd-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfdfd-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cfdfd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfdfd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfdfd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfdfd-115">Not supported.</span></span>|
|<span data-ttu-id="cfdfd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cfdfd-116">Application</span></span>|<span data-ttu-id="cfdfd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfdfd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfdfd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfdfd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="cfdfd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfdfd-119">Request headers</span></span>
|<span data-ttu-id="cfdfd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cfdfd-120">Header</span></span>|<span data-ttu-id="cfdfd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cfdfd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfdfd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfdfd-122">Authorization</span></span>|<span data-ttu-id="cfdfd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfdfd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfdfd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cfdfd-124">Accept</span></span>|<span data-ttu-id="cfdfd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cfdfd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfdfd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfdfd-126">Request body</span></span>
<span data-ttu-id="cfdfd-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="cfdfd-127">In the request body, supply a JSON representation for the groupPolicyConfigurationAssignment object.</span></span>

<span data-ttu-id="cfdfd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="cfdfd-128">The following table shows the properties that are required when you create the groupPolicyConfigurationAssignment.</span></span>

|<span data-ttu-id="cfdfd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfdfd-129">Property</span></span>|<span data-ttu-id="cfdfd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfdfd-130">Type</span></span>|<span data-ttu-id="cfdfd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfdfd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfdfd-132">id</span><span class="sxs-lookup"><span data-stu-id="cfdfd-132">id</span></span>|<span data-ttu-id="cfdfd-133">String</span><span class="sxs-lookup"><span data-stu-id="cfdfd-133">String</span></span>|<span data-ttu-id="cfdfd-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cfdfd-134">Key of the entity.</span></span>|
|<span data-ttu-id="cfdfd-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cfdfd-135">lastModifiedDateTime</span></span>|<span data-ttu-id="cfdfd-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfdfd-136">DateTimeOffset</span></span>|<span data-ttu-id="cfdfd-137">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cfdfd-137">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="cfdfd-138">destino</span><span class="sxs-lookup"><span data-stu-id="cfdfd-138">target</span></span>|[<span data-ttu-id="cfdfd-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cfdfd-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cfdfd-140">O tipo de grupo de destino da configuração da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="cfdfd-140">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="cfdfd-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfdfd-141">Response</span></span>
<span data-ttu-id="cfdfd-142">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfdfd-142">If successful, this method returns a `201 Created` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfdfd-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cfdfd-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfdfd-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfdfd-144">Request</span></span>
<span data-ttu-id="cfdfd-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfdfd-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="cfdfd-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfdfd-146">Response</span></span>
<span data-ttu-id="cfdfd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfdfd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```






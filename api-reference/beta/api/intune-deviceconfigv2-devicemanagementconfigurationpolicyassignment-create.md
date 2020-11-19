---
title: Criar deviceManagementConfigurationPolicyAssignment
description: Criar um novo objeto deviceManagementConfigurationPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fdacc5f360340e6e07de25183ed53ddce181b15e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301463"
---
# <a name="create-devicemanagementconfigurationpolicyassignment"></a><span data-ttu-id="6d6b7-103">Criar deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="6d6b7-103">Create deviceManagementConfigurationPolicyAssignment</span></span>

<span data-ttu-id="6d6b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d6b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d6b7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d6b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d6b7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d6b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d6b7-107">Criar um novo objeto [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6d6b7-107">Create a new [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d6b7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6d6b7-108">Prerequisites</span></span>
<span data-ttu-id="6d6b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d6b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d6b7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d6b7-111">Permission type</span></span>|<span data-ttu-id="6d6b7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6d6b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d6b7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d6b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d6b7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d6b7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6d6b7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d6b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d6b7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d6b7-116">Not supported.</span></span>|
|<span data-ttu-id="6d6b7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d6b7-117">Application</span></span>|<span data-ttu-id="6d6b7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d6b7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d6b7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d6b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6d6b7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d6b7-120">Request headers</span></span>
|<span data-ttu-id="6d6b7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d6b7-121">Header</span></span>|<span data-ttu-id="6d6b7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6d6b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d6b7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d6b7-123">Authorization</span></span>|<span data-ttu-id="6d6b7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d6b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d6b7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d6b7-125">Accept</span></span>|<span data-ttu-id="6d6b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d6b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d6b7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d6b7-127">Request body</span></span>
<span data-ttu-id="6d6b7-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementConfigurationPolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="6d6b7-128">In the request body, supply a JSON representation for the deviceManagementConfigurationPolicyAssignment object.</span></span>

<span data-ttu-id="6d6b7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationPolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="6d6b7-129">The following table shows the properties that are required when you create the deviceManagementConfigurationPolicyAssignment.</span></span>

|<span data-ttu-id="6d6b7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d6b7-130">Property</span></span>|<span data-ttu-id="6d6b7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d6b7-131">Type</span></span>|<span data-ttu-id="6d6b7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d6b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d6b7-133">id</span><span class="sxs-lookup"><span data-stu-id="6d6b7-133">id</span></span>|<span data-ttu-id="6d6b7-134">String</span><span class="sxs-lookup"><span data-stu-id="6d6b7-134">String</span></span>|<span data-ttu-id="6d6b7-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="6d6b7-135">The key of the assignment.</span></span>|
|<span data-ttu-id="6d6b7-136">destino</span><span class="sxs-lookup"><span data-stu-id="6d6b7-136">target</span></span>|[<span data-ttu-id="6d6b7-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6d6b7-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6d6b7-138">O destino de atribuição para o DeviceManagementConfigurationPolicy.</span><span class="sxs-lookup"><span data-stu-id="6d6b7-138">The assignment target for the DeviceManagementConfigurationPolicy.</span></span>|



## <a name="response"></a><span data-ttu-id="6d6b7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d6b7-139">Response</span></span>
<span data-ttu-id="6d6b7-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d6b7-140">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d6b7-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d6b7-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d6b7-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d6b7-142">Request</span></span>
<span data-ttu-id="6d6b7-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d6b7-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments
Content-type: application/json
Content-length: 340

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="6d6b7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d6b7-144">Response</span></span>
<span data-ttu-id="6d6b7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d6b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 389

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "id": "1f069921-9921-1f06-2199-061f2199061f",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```





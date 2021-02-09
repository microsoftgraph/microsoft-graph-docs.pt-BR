---
title: Atualizar deviceManagementConfigurationPolicyAssignment
description: Atualizar as propriedades de um objeto deviceManagementConfigurationPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 621aea837fc8db819d4f20855bc9393755283dbf
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155696"
---
# <a name="update-devicemanagementconfigurationpolicyassignment"></a><span data-ttu-id="b702c-103">Atualizar deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="b702c-103">Update deviceManagementConfigurationPolicyAssignment</span></span>

<span data-ttu-id="b702c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b702c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b702c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b702c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b702c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b702c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b702c-107">Atualizar as propriedades de um [objeto deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b702c-107">Update the properties of a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b702c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b702c-108">Prerequisites</span></span>
<span data-ttu-id="b702c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b702c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b702c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b702c-111">Permission type</span></span>|<span data-ttu-id="b702c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b702c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b702c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b702c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b702c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b702c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b702c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b702c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b702c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b702c-116">Not supported.</span></span>|
|<span data-ttu-id="b702c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b702c-117">Application</span></span>|<span data-ttu-id="b702c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b702c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b702c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b702c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments/{deviceManagementConfigurationPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b702c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b702c-120">Request headers</span></span>
|<span data-ttu-id="b702c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b702c-121">Header</span></span>|<span data-ttu-id="b702c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b702c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b702c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b702c-123">Authorization</span></span>|<span data-ttu-id="b702c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b702c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b702c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b702c-125">Accept</span></span>|<span data-ttu-id="b702c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b702c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b702c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b702c-127">Request body</span></span>
<span data-ttu-id="b702c-128">No corpo da solicitação, fornece uma representação JSON do [objeto deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b702c-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>

<span data-ttu-id="b702c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b702c-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md).</span></span>

|<span data-ttu-id="b702c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b702c-130">Property</span></span>|<span data-ttu-id="b702c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b702c-131">Type</span></span>|<span data-ttu-id="b702c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b702c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b702c-133">id</span><span class="sxs-lookup"><span data-stu-id="b702c-133">id</span></span>|<span data-ttu-id="b702c-134">String</span><span class="sxs-lookup"><span data-stu-id="b702c-134">String</span></span>|<span data-ttu-id="b702c-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="b702c-135">The key of the assignment.</span></span>|
|<span data-ttu-id="b702c-136">destino</span><span class="sxs-lookup"><span data-stu-id="b702c-136">target</span></span>|[<span data-ttu-id="b702c-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b702c-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b702c-138">O destino de atribuição para DeviceManagementConfigurationPolicy.</span><span class="sxs-lookup"><span data-stu-id="b702c-138">The assignment target for the DeviceManagementConfigurationPolicy.</span></span>|



## <a name="response"></a><span data-ttu-id="b702c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b702c-139">Response</span></span>
<span data-ttu-id="b702c-140">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b702c-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b702c-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b702c-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b702c-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b702c-142">Request</span></span>
<span data-ttu-id="b702c-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b702c-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments/{deviceManagementConfigurationPolicyAssignmentId}
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="b702c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b702c-144">Response</span></span>
<span data-ttu-id="b702c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b702c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "id": "1f069921-9921-1f06-2199-061f2199061f",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```





---
title: Criar groupPolicyConfigurationAssignment
description: Criar um novo objeto groupPolicyConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d6fb517a5803c06144104116a55a26e3d246e68d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155024"
---
# <a name="create-grouppolicyconfigurationassignment"></a><span data-ttu-id="ba2b5-103">Criar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ba2b5-103">Create groupPolicyConfigurationAssignment</span></span>

<span data-ttu-id="ba2b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba2b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba2b5-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ba2b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba2b5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba2b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba2b5-107">Criar um novo [objeto groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ba2b5-107">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba2b5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ba2b5-108">Prerequisites</span></span>
<span data-ttu-id="ba2b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba2b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba2b5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba2b5-111">Permission type</span></span>|<span data-ttu-id="ba2b5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ba2b5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba2b5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba2b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba2b5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba2b5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ba2b5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba2b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba2b5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba2b5-116">Not supported.</span></span>|
|<span data-ttu-id="ba2b5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba2b5-117">Application</span></span>|<span data-ttu-id="ba2b5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba2b5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba2b5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba2b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ba2b5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba2b5-120">Request headers</span></span>
|<span data-ttu-id="ba2b5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba2b5-121">Header</span></span>|<span data-ttu-id="ba2b5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ba2b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba2b5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba2b5-123">Authorization</span></span>|<span data-ttu-id="ba2b5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba2b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba2b5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ba2b5-125">Accept</span></span>|<span data-ttu-id="ba2b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba2b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba2b5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba2b5-127">Request body</span></span>
<span data-ttu-id="ba2b5-128">No corpo da solicitação, fornece uma representação JSON do objeto groupPolicyConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="ba2b5-128">In the request body, supply a JSON representation for the groupPolicyConfigurationAssignment object.</span></span>

<span data-ttu-id="ba2b5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="ba2b5-129">The following table shows the properties that are required when you create the groupPolicyConfigurationAssignment.</span></span>

|<span data-ttu-id="ba2b5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba2b5-130">Property</span></span>|<span data-ttu-id="ba2b5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba2b5-131">Type</span></span>|<span data-ttu-id="ba2b5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba2b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba2b5-133">id</span><span class="sxs-lookup"><span data-stu-id="ba2b5-133">id</span></span>|<span data-ttu-id="ba2b5-134">String</span><span class="sxs-lookup"><span data-stu-id="ba2b5-134">String</span></span>|<span data-ttu-id="ba2b5-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ba2b5-135">Key of the entity.</span></span>|
|<span data-ttu-id="ba2b5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba2b5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ba2b5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba2b5-137">DateTimeOffset</span></span>|<span data-ttu-id="ba2b5-138">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ba2b5-138">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="ba2b5-139">destino</span><span class="sxs-lookup"><span data-stu-id="ba2b5-139">target</span></span>|[<span data-ttu-id="ba2b5-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ba2b5-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ba2b5-141">O tipo de grupos direcionados à configuração da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="ba2b5-141">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="ba2b5-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba2b5-142">Response</span></span>
<span data-ttu-id="ba2b5-143">Se tiver êxito, este método retornará um código de resposta e um objeto `201 Created` [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba2b5-143">If successful, this method returns a `201 Created` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba2b5-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba2b5-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba2b5-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba2b5-145">Request</span></span>
<span data-ttu-id="ba2b5-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba2b5-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
Content-type: application/json
Content-length: 393

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="ba2b5-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba2b5-147">Response</span></span>
<span data-ttu-id="ba2b5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba2b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 506

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```





---
title: Atualizar groupPolicyConfigurationAssignment
description: Atualize as propriedades de um objeto groupPolicyConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d238abe2f3ade6b9dcbc54b4e5fb9867f53c6ce2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135450"
---
# <a name="update-grouppolicyconfigurationassignment"></a><span data-ttu-id="c9200-103">Atualizar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c9200-103">Update groupPolicyConfigurationAssignment</span></span>

<span data-ttu-id="c9200-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9200-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9200-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c9200-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9200-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c9200-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9200-107">Atualize as propriedades de [um objeto groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c9200-107">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9200-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c9200-108">Prerequisites</span></span>
<span data-ttu-id="c9200-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9200-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9200-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9200-111">Permission type</span></span>|<span data-ttu-id="c9200-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9200-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9200-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9200-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9200-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9200-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9200-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9200-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9200-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9200-116">Not supported.</span></span>|
|<span data-ttu-id="c9200-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9200-117">Application</span></span>|<span data-ttu-id="c9200-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9200-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9200-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9200-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c9200-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9200-120">Request headers</span></span>
|<span data-ttu-id="c9200-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9200-121">Header</span></span>|<span data-ttu-id="c9200-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c9200-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9200-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9200-123">Authorization</span></span>|<span data-ttu-id="c9200-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9200-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9200-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c9200-125">Accept</span></span>|<span data-ttu-id="c9200-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9200-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9200-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9200-127">Request body</span></span>
<span data-ttu-id="c9200-128">No corpo da solicitação, fornece uma representação JSON para o [objeto groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c9200-128">In the request body, supply a JSON representation for the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

<span data-ttu-id="c9200-129">A tabela a seguir mostra as propriedades necessárias ao criar [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c9200-129">The following table shows the properties that are required when you create the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>

|<span data-ttu-id="c9200-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9200-130">Property</span></span>|<span data-ttu-id="c9200-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9200-131">Type</span></span>|<span data-ttu-id="c9200-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9200-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9200-133">id</span><span class="sxs-lookup"><span data-stu-id="c9200-133">id</span></span>|<span data-ttu-id="c9200-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9200-134">String</span></span>|<span data-ttu-id="c9200-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c9200-135">Key of the entity.</span></span>|
|<span data-ttu-id="c9200-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9200-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c9200-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9200-137">DateTimeOffset</span></span>|<span data-ttu-id="c9200-138">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c9200-138">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="c9200-139">destino</span><span class="sxs-lookup"><span data-stu-id="c9200-139">target</span></span>|[<span data-ttu-id="c9200-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c9200-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c9200-141">O tipo de grupos direcionados à configuração da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="c9200-141">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="c9200-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9200-142">Response</span></span>
<span data-ttu-id="c9200-143">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9200-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9200-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9200-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9200-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9200-145">Request</span></span>
<span data-ttu-id="c9200-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9200-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
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

### <a name="response"></a><span data-ttu-id="c9200-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9200-147">Response</span></span>
<span data-ttu-id="c9200-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9200-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





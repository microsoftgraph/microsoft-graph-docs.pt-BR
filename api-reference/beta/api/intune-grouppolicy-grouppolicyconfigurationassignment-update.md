---
title: Atualizar groupPolicyConfigurationAssignment
description: Atualiza as propriedades de um objeto groupPolicyConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 097c7a828dfabb040ddf2dc27683f47d0dc75797
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37179800"
---
# <a name="update-grouppolicyconfigurationassignment"></a><span data-ttu-id="fec66-103">Atualizar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="fec66-103">Update groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="fec66-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fec66-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fec66-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fec66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fec66-106">Atualiza as propriedades de um objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="fec66-106">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fec66-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fec66-107">Prerequisites</span></span>
<span data-ttu-id="fec66-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fec66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fec66-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fec66-110">Permission type</span></span>|<span data-ttu-id="fec66-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fec66-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fec66-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fec66-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fec66-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fec66-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fec66-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fec66-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fec66-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fec66-115">Not supported.</span></span>|
|<span data-ttu-id="fec66-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fec66-116">Application</span></span>|<span data-ttu-id="fec66-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fec66-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fec66-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fec66-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="fec66-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fec66-119">Request headers</span></span>
|<span data-ttu-id="fec66-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fec66-120">Header</span></span>|<span data-ttu-id="fec66-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fec66-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fec66-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fec66-122">Authorization</span></span>|<span data-ttu-id="fec66-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fec66-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fec66-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fec66-124">Accept</span></span>|<span data-ttu-id="fec66-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fec66-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fec66-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fec66-126">Request body</span></span>
<span data-ttu-id="fec66-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="fec66-127">In the request body, supply a JSON representation for the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

<span data-ttu-id="fec66-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fec66-128">The following table shows the properties that are required when you create the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>

|<span data-ttu-id="fec66-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fec66-129">Property</span></span>|<span data-ttu-id="fec66-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fec66-130">Type</span></span>|<span data-ttu-id="fec66-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fec66-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fec66-132">id</span><span class="sxs-lookup"><span data-stu-id="fec66-132">id</span></span>|<span data-ttu-id="fec66-133">String</span><span class="sxs-lookup"><span data-stu-id="fec66-133">String</span></span>|<span data-ttu-id="fec66-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fec66-134">Key of the entity.</span></span>|
|<span data-ttu-id="fec66-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fec66-135">lastModifiedDateTime</span></span>|<span data-ttu-id="fec66-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fec66-136">DateTimeOffset</span></span>|<span data-ttu-id="fec66-137">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fec66-137">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="fec66-138">destino</span><span class="sxs-lookup"><span data-stu-id="fec66-138">target</span></span>|[<span data-ttu-id="fec66-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fec66-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fec66-140">O tipo de grupo de destino da configuração da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="fec66-140">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="fec66-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="fec66-141">Response</span></span>
<span data-ttu-id="fec66-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fec66-142">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fec66-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fec66-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="fec66-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fec66-144">Request</span></span>
<span data-ttu-id="fec66-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fec66-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="fec66-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="fec66-146">Response</span></span>
<span data-ttu-id="fec66-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fec66-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





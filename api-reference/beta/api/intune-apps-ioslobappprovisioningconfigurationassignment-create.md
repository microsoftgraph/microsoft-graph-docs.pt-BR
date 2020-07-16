---
title: Criar iosLobAppProvisioningConfigurationAssignment
description: Criar um novo objeto iosLobAppProvisioningConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a061f97491ea006d2655ef2caa9e8c6e78f185c0
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793399"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="848e9-103">Criar iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="848e9-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

<span data-ttu-id="848e9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="848e9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="848e9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="848e9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="848e9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="848e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="848e9-107">Criar um novo objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="848e9-107">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="848e9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="848e9-108">Prerequisites</span></span>
<span data-ttu-id="848e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="848e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="848e9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="848e9-111">Permission type</span></span>|<span data-ttu-id="848e9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="848e9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="848e9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="848e9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="848e9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="848e9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="848e9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="848e9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="848e9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="848e9-116">Not supported.</span></span>|
|<span data-ttu-id="848e9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="848e9-117">Application</span></span>|<span data-ttu-id="848e9-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="848e9-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="848e9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="848e9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="848e9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="848e9-120">Request headers</span></span>
|<span data-ttu-id="848e9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="848e9-121">Header</span></span>|<span data-ttu-id="848e9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="848e9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="848e9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="848e9-123">Authorization</span></span>|<span data-ttu-id="848e9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="848e9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="848e9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="848e9-125">Accept</span></span>|<span data-ttu-id="848e9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="848e9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="848e9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="848e9-127">Request body</span></span>
<span data-ttu-id="848e9-128">No corpo da solicitação, forneça uma representação JSON do objeto iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="848e9-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="848e9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="848e9-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="848e9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="848e9-130">Property</span></span>|<span data-ttu-id="848e9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="848e9-131">Type</span></span>|<span data-ttu-id="848e9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="848e9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="848e9-133">id</span><span class="sxs-lookup"><span data-stu-id="848e9-133">id</span></span>|<span data-ttu-id="848e9-134">String</span><span class="sxs-lookup"><span data-stu-id="848e9-134">String</span></span>|<span data-ttu-id="848e9-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="848e9-135">Key of the entity.</span></span>|
|<span data-ttu-id="848e9-136">destino</span><span class="sxs-lookup"><span data-stu-id="848e9-136">target</span></span>|[<span data-ttu-id="848e9-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="848e9-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="848e9-138">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="848e9-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="848e9-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="848e9-139">Response</span></span>
<span data-ttu-id="848e9-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="848e9-140">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="848e9-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="848e9-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="848e9-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="848e9-142">Request</span></span>
<span data-ttu-id="848e9-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="848e9-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
Content-type: application/json
Content-length: 351

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="848e9-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="848e9-144">Response</span></span>
<span data-ttu-id="848e9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="848e9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 400

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




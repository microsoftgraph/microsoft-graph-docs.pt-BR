---
title: Atualizar iosLobAppProvisioningConfigurationAssignment
description: Atualiza as propriedades de um objeto iosLobAppProvisioningConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8f0bdd5ac80c537f3908964b17f2c88ec0db6583
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43394990"
---
# <a name="update-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="e9e77-103">Atualizar iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e9e77-103">Update iosLobAppProvisioningConfigurationAssignment</span></span>

<span data-ttu-id="e9e77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9e77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9e77-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e9e77-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9e77-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9e77-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9e77-107">Atualiza as propriedades de um objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e9e77-107">Update the properties of a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9e77-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9e77-108">Prerequisites</span></span>
<span data-ttu-id="e9e77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9e77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9e77-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9e77-111">Permission type</span></span>|<span data-ttu-id="e9e77-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e9e77-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9e77-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9e77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9e77-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9e77-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e9e77-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9e77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9e77-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9e77-116">Not supported.</span></span>|
|<span data-ttu-id="e9e77-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9e77-117">Application</span></span>|<span data-ttu-id="e9e77-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9e77-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9e77-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9e77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e9e77-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9e77-120">Request headers</span></span>
|<span data-ttu-id="e9e77-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9e77-121">Header</span></span>|<span data-ttu-id="e9e77-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e9e77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9e77-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9e77-123">Authorization</span></span>|<span data-ttu-id="e9e77-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9e77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9e77-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9e77-125">Accept</span></span>|<span data-ttu-id="e9e77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9e77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9e77-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9e77-127">Request body</span></span>
<span data-ttu-id="e9e77-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e9e77-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

<span data-ttu-id="e9e77-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e9e77-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

|<span data-ttu-id="e9e77-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9e77-130">Property</span></span>|<span data-ttu-id="e9e77-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9e77-131">Type</span></span>|<span data-ttu-id="e9e77-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9e77-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9e77-133">id</span><span class="sxs-lookup"><span data-stu-id="e9e77-133">id</span></span>|<span data-ttu-id="e9e77-134">String</span><span class="sxs-lookup"><span data-stu-id="e9e77-134">String</span></span>|<span data-ttu-id="e9e77-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e9e77-135">Key of the entity.</span></span>|
|<span data-ttu-id="e9e77-136">destino</span><span class="sxs-lookup"><span data-stu-id="e9e77-136">target</span></span>|[<span data-ttu-id="e9e77-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e9e77-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e9e77-138">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e9e77-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="e9e77-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9e77-139">Response</span></span>
<span data-ttu-id="e9e77-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9e77-140">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9e77-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9e77-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9e77-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9e77-142">Request</span></span>
<span data-ttu-id="e9e77-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9e77-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e9e77-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9e77-144">Response</span></span>
<span data-ttu-id="e9e77-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9e77-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




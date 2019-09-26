---
title: Criar iosLobAppProvisioningConfigurationAssignment
description: Criar um novo objeto iosLobAppProvisioningConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1cbc6ac636628706f7da320f24404770c02fc7f3
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37177896"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="2a084-103">Criar iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a084-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="2a084-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2a084-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a084-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2a084-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a084-106">Criar um novo objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2a084-106">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a084-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2a084-107">Prerequisites</span></span>
<span data-ttu-id="2a084-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a084-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a084-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a084-110">Permission type</span></span>|<span data-ttu-id="2a084-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2a084-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a084-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a084-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a084-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a084-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2a084-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a084-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a084-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a084-115">Not supported.</span></span>|
|<span data-ttu-id="2a084-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a084-116">Application</span></span>|<span data-ttu-id="2a084-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a084-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a084-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a084-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2a084-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a084-119">Request headers</span></span>
|<span data-ttu-id="2a084-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a084-120">Header</span></span>|<span data-ttu-id="2a084-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2a084-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a084-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a084-122">Authorization</span></span>|<span data-ttu-id="2a084-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a084-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a084-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2a084-124">Accept</span></span>|<span data-ttu-id="2a084-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a084-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a084-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a084-126">Request body</span></span>
<span data-ttu-id="2a084-127">No corpo da solicitação, forneça uma representação JSON do objeto iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="2a084-127">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="2a084-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="2a084-128">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="2a084-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a084-129">Property</span></span>|<span data-ttu-id="2a084-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a084-130">Type</span></span>|<span data-ttu-id="2a084-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a084-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a084-132">id</span><span class="sxs-lookup"><span data-stu-id="2a084-132">id</span></span>|<span data-ttu-id="2a084-133">String</span><span class="sxs-lookup"><span data-stu-id="2a084-133">String</span></span>|<span data-ttu-id="2a084-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2a084-134">Key of the entity.</span></span>|
|<span data-ttu-id="2a084-135">destino</span><span class="sxs-lookup"><span data-stu-id="2a084-135">target</span></span>|[<span data-ttu-id="2a084-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2a084-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2a084-137">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="2a084-137">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="2a084-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a084-138">Response</span></span>
<span data-ttu-id="2a084-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a084-139">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a084-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a084-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a084-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a084-141">Request</span></span>
<span data-ttu-id="2a084-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a084-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="2a084-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a084-143">Response</span></span>
<span data-ttu-id="2a084-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a084-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





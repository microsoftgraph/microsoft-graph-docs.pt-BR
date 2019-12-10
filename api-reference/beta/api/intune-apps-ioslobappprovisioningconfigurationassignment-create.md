---
title: Criar iosLobAppProvisioningConfigurationAssignment
description: Criar um novo objeto iosLobAppProvisioningConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8eb329ea455dacd28d769dd7e1734d0e2a745b34
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39921309"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="95783-103">Criar iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="95783-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="95783-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="95783-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95783-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95783-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95783-106">Criar um novo objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="95783-106">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95783-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="95783-107">Prerequisites</span></span>
<span data-ttu-id="95783-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95783-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95783-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95783-110">Permission type</span></span>|<span data-ttu-id="95783-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="95783-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95783-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95783-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95783-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95783-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="95783-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95783-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95783-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95783-115">Not supported.</span></span>|
|<span data-ttu-id="95783-116">Application</span><span class="sxs-lookup"><span data-stu-id="95783-116">Application</span></span>|<span data-ttu-id="95783-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95783-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95783-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95783-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="95783-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95783-119">Request headers</span></span>
|<span data-ttu-id="95783-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95783-120">Header</span></span>|<span data-ttu-id="95783-121">Valor</span><span class="sxs-lookup"><span data-stu-id="95783-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95783-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="95783-122">Authorization</span></span>|<span data-ttu-id="95783-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95783-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95783-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="95783-124">Accept</span></span>|<span data-ttu-id="95783-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95783-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95783-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95783-126">Request body</span></span>
<span data-ttu-id="95783-127">No corpo da solicitação, forneça uma representação JSON do objeto iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="95783-127">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="95783-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="95783-128">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="95783-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95783-129">Property</span></span>|<span data-ttu-id="95783-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="95783-130">Type</span></span>|<span data-ttu-id="95783-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="95783-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95783-132">id</span><span class="sxs-lookup"><span data-stu-id="95783-132">id</span></span>|<span data-ttu-id="95783-133">String</span><span class="sxs-lookup"><span data-stu-id="95783-133">String</span></span>|<span data-ttu-id="95783-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="95783-134">Key of the entity.</span></span>|
|<span data-ttu-id="95783-135">destino</span><span class="sxs-lookup"><span data-stu-id="95783-135">target</span></span>|[<span data-ttu-id="95783-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="95783-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="95783-137">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="95783-137">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="95783-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="95783-138">Response</span></span>
<span data-ttu-id="95783-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95783-139">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95783-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95783-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="95783-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95783-141">Request</span></span>
<span data-ttu-id="95783-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95783-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="95783-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="95783-143">Response</span></span>
<span data-ttu-id="95783-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95783-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






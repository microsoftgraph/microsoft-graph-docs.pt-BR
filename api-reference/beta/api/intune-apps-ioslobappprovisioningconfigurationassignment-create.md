---
title: Criar iosLobAppProvisioningConfigurationAssignment
description: Criar um novo objeto iosLobAppProvisioningConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9d2af6426c1449e1680bfa0b789972d372584af0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445712"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="f354a-103">Criar iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f354a-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

<span data-ttu-id="f354a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f354a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f354a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f354a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f354a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f354a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f354a-107">Criar um novo objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="f354a-107">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f354a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f354a-108">Prerequisites</span></span>
<span data-ttu-id="f354a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f354a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f354a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f354a-111">Permission type</span></span>|<span data-ttu-id="f354a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f354a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f354a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f354a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f354a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f354a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f354a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f354a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f354a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f354a-116">Not supported.</span></span>|
|<span data-ttu-id="f354a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f354a-117">Application</span></span>|<span data-ttu-id="f354a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f354a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f354a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f354a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f354a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f354a-120">Request headers</span></span>
|<span data-ttu-id="f354a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f354a-121">Header</span></span>|<span data-ttu-id="f354a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f354a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f354a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f354a-123">Authorization</span></span>|<span data-ttu-id="f354a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f354a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f354a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f354a-125">Accept</span></span>|<span data-ttu-id="f354a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f354a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f354a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f354a-127">Request body</span></span>
<span data-ttu-id="f354a-128">No corpo da solicitação, forneça uma representação JSON do objeto iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="f354a-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="f354a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="f354a-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="f354a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f354a-130">Property</span></span>|<span data-ttu-id="f354a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f354a-131">Type</span></span>|<span data-ttu-id="f354a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f354a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f354a-133">id</span><span class="sxs-lookup"><span data-stu-id="f354a-133">id</span></span>|<span data-ttu-id="f354a-134">String</span><span class="sxs-lookup"><span data-stu-id="f354a-134">String</span></span>|<span data-ttu-id="f354a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f354a-135">Key of the entity.</span></span>|
|<span data-ttu-id="f354a-136">destino</span><span class="sxs-lookup"><span data-stu-id="f354a-136">target</span></span>|[<span data-ttu-id="f354a-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f354a-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f354a-138">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f354a-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="f354a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f354a-139">Response</span></span>
<span data-ttu-id="f354a-140">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f354a-140">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f354a-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f354a-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="f354a-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f354a-142">Request</span></span>
<span data-ttu-id="f354a-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f354a-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f354a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f354a-144">Response</span></span>
<span data-ttu-id="f354a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f354a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






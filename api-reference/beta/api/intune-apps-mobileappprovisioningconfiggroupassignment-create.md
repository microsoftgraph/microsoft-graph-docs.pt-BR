---
title: Criar mobileAppProvisioningConfigGroupAssignment
description: Criar um novo objeto mobileAppProvisioningConfigGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4cd6ee5c224756aaaf4e98657c7fda4061f8c101
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37172496"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="50f39-103">Criar mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="50f39-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="50f39-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50f39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50f39-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50f39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50f39-106">Criar um novo objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="50f39-106">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50f39-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50f39-107">Prerequisites</span></span>
<span data-ttu-id="50f39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50f39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50f39-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50f39-110">Permission type</span></span>|<span data-ttu-id="50f39-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50f39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50f39-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50f39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50f39-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50f39-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="50f39-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50f39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50f39-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50f39-115">Not supported.</span></span>|
|<span data-ttu-id="50f39-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50f39-116">Application</span></span>|<span data-ttu-id="50f39-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50f39-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50f39-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50f39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="50f39-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50f39-119">Request headers</span></span>
|<span data-ttu-id="50f39-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50f39-120">Header</span></span>|<span data-ttu-id="50f39-121">Valor</span><span class="sxs-lookup"><span data-stu-id="50f39-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50f39-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="50f39-122">Authorization</span></span>|<span data-ttu-id="50f39-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50f39-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50f39-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50f39-124">Accept</span></span>|<span data-ttu-id="50f39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="50f39-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50f39-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50f39-126">Request body</span></span>
<span data-ttu-id="50f39-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppProvisioningConfigGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="50f39-127">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="50f39-128">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppProvisioningConfigGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="50f39-128">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="50f39-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50f39-129">Property</span></span>|<span data-ttu-id="50f39-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="50f39-130">Type</span></span>|<span data-ttu-id="50f39-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="50f39-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50f39-132">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="50f39-132">targetGroupId</span></span>|<span data-ttu-id="50f39-133">String</span><span class="sxs-lookup"><span data-stu-id="50f39-133">String</span></span>|<span data-ttu-id="50f39-134">A ID do grupo do AAD no qual a configuração de provisionamento do aplicativo está sendo direcionada.</span><span class="sxs-lookup"><span data-stu-id="50f39-134">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="50f39-135">id</span><span class="sxs-lookup"><span data-stu-id="50f39-135">id</span></span>|<span data-ttu-id="50f39-136">String</span><span class="sxs-lookup"><span data-stu-id="50f39-136">String</span></span>|<span data-ttu-id="50f39-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="50f39-137">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="50f39-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="50f39-138">Response</span></span>
<span data-ttu-id="50f39-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50f39-139">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50f39-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50f39-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="50f39-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50f39-141">Request</span></span>
<span data-ttu-id="50f39-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50f39-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="50f39-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="50f39-143">Response</span></span>
<span data-ttu-id="50f39-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50f39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```





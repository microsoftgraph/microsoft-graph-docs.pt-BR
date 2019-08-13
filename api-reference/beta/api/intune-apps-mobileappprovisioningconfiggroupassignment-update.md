---
title: Atualizar mobileAppProvisioningConfigGroupAssignment
description: Atualiza as propriedades de um objeto mobileAppProvisioningConfigGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 21b9737de279ec0d6444e2cd2b6b44cb9e6123da
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329065"
---
# <a name="update-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="91ff3-103">Atualizar mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="91ff3-103">Update mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="91ff3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="91ff3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91ff3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91ff3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91ff3-106">Atualiza as propriedades de um objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="91ff3-106">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91ff3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91ff3-107">Prerequisites</span></span>
<span data-ttu-id="91ff3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91ff3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91ff3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91ff3-110">Permission type</span></span>|<span data-ttu-id="91ff3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="91ff3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91ff3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91ff3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91ff3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91ff3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="91ff3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91ff3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91ff3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91ff3-115">Not supported.</span></span>|
|<span data-ttu-id="91ff3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91ff3-116">Application</span></span>|<span data-ttu-id="91ff3-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91ff3-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91ff3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91ff3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="91ff3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91ff3-119">Request headers</span></span>
|<span data-ttu-id="91ff3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91ff3-120">Header</span></span>|<span data-ttu-id="91ff3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="91ff3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91ff3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="91ff3-122">Authorization</span></span>|<span data-ttu-id="91ff3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91ff3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91ff3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="91ff3-124">Accept</span></span>|<span data-ttu-id="91ff3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="91ff3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91ff3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91ff3-126">Request body</span></span>
<span data-ttu-id="91ff3-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="91ff3-127">In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

<span data-ttu-id="91ff3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="91ff3-128">The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

|<span data-ttu-id="91ff3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91ff3-129">Property</span></span>|<span data-ttu-id="91ff3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="91ff3-130">Type</span></span>|<span data-ttu-id="91ff3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="91ff3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91ff3-132">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="91ff3-132">targetGroupId</span></span>|<span data-ttu-id="91ff3-133">String</span><span class="sxs-lookup"><span data-stu-id="91ff3-133">String</span></span>|<span data-ttu-id="91ff3-134">A ID do grupo do AAD no qual a configuração de provisionamento do aplicativo está sendo direcionada.</span><span class="sxs-lookup"><span data-stu-id="91ff3-134">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="91ff3-135">id</span><span class="sxs-lookup"><span data-stu-id="91ff3-135">id</span></span>|<span data-ttu-id="91ff3-136">String</span><span class="sxs-lookup"><span data-stu-id="91ff3-136">String</span></span>|<span data-ttu-id="91ff3-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="91ff3-137">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="91ff3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="91ff3-138">Response</span></span>
<span data-ttu-id="91ff3-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91ff3-139">If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91ff3-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91ff3-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="91ff3-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91ff3-141">Request</span></span>
<span data-ttu-id="91ff3-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91ff3-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="91ff3-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="91ff3-143">Response</span></span>
<span data-ttu-id="91ff3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91ff3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```







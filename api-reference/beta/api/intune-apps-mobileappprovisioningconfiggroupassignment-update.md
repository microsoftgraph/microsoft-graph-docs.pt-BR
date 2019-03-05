---
title: Atualizar mobileAppProvisioningConfigGroupAssignment
description: Atualiza as propriedades de um objeto mobileAppProvisioningConfigGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 21c4c65dc6deec19cda232d4c5be377e38e92a9a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144398"
---
# <a name="update-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="51b09-103">Atualizar mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="51b09-103">Update mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="51b09-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="51b09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51b09-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51b09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51b09-106">Atualiza as propriedades de um objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="51b09-106">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51b09-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51b09-107">Prerequisites</span></span>
<span data-ttu-id="51b09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="51b09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="51b09-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51b09-110">Permission type</span></span>|<span data-ttu-id="51b09-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51b09-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51b09-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51b09-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51b09-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51b09-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51b09-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51b09-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51b09-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51b09-115">Not supported.</span></span>|
|<span data-ttu-id="51b09-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51b09-116">Application</span></span>|<span data-ttu-id="51b09-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51b09-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51b09-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51b09-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="51b09-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51b09-119">Request headers</span></span>
|<span data-ttu-id="51b09-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51b09-120">Header</span></span>|<span data-ttu-id="51b09-121">Valor</span><span class="sxs-lookup"><span data-stu-id="51b09-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51b09-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="51b09-122">Authorization</span></span>|<span data-ttu-id="51b09-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51b09-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51b09-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51b09-124">Accept</span></span>|<span data-ttu-id="51b09-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51b09-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51b09-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51b09-126">Request body</span></span>
<span data-ttu-id="51b09-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="51b09-127">In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

<span data-ttu-id="51b09-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="51b09-128">The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

|<span data-ttu-id="51b09-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51b09-129">Property</span></span>|<span data-ttu-id="51b09-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="51b09-130">Type</span></span>|<span data-ttu-id="51b09-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="51b09-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51b09-132">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="51b09-132">targetGroupId</span></span>|<span data-ttu-id="51b09-133">String</span><span class="sxs-lookup"><span data-stu-id="51b09-133">String</span></span>|<span data-ttu-id="51b09-134">A ID do grupo do AAD no qual a configuração de provisionamento do aplicativo está sendo direcionada.</span><span class="sxs-lookup"><span data-stu-id="51b09-134">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="51b09-135">id</span><span class="sxs-lookup"><span data-stu-id="51b09-135">id</span></span>|<span data-ttu-id="51b09-136">String</span><span class="sxs-lookup"><span data-stu-id="51b09-136">String</span></span>|<span data-ttu-id="51b09-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="51b09-137">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="51b09-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="51b09-138">Response</span></span>
<span data-ttu-id="51b09-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51b09-139">If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51b09-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51b09-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="51b09-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51b09-141">Request</span></span>
<span data-ttu-id="51b09-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51b09-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="51b09-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="51b09-143">Response</span></span>
<span data-ttu-id="51b09-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51b09-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





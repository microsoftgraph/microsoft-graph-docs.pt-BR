---
title: Atualizar mobileAppProvisioningConfigGroupAssignment
description: Atualiza as propriedades de um objeto mobileAppProvisioningConfigGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 73f169fd214a694f1b0bdd3da9b47602cf412523
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724393"
---
# <a name="update-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="e5d84-103">Atualizar mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="e5d84-103">Update mobileAppProvisioningConfigGroupAssignment</span></span>

<span data-ttu-id="e5d84-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5d84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5d84-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e5d84-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5d84-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5d84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5d84-107">Atualiza as propriedades de um objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e5d84-107">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5d84-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e5d84-108">Prerequisites</span></span>
<span data-ttu-id="e5d84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5d84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5d84-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5d84-111">Permission type</span></span>|<span data-ttu-id="e5d84-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e5d84-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5d84-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5d84-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5d84-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5d84-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e5d84-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5d84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5d84-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5d84-116">Not supported.</span></span>|
|<span data-ttu-id="e5d84-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5d84-117">Application</span></span>|<span data-ttu-id="e5d84-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5d84-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5d84-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5d84-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e5d84-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5d84-120">Request headers</span></span>
|<span data-ttu-id="e5d84-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e5d84-121">Header</span></span>|<span data-ttu-id="e5d84-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e5d84-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5d84-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5d84-123">Authorization</span></span>|<span data-ttu-id="e5d84-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5d84-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5d84-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e5d84-125">Accept</span></span>|<span data-ttu-id="e5d84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5d84-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5d84-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5d84-127">Request body</span></span>
<span data-ttu-id="e5d84-128">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e5d84-128">In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

<span data-ttu-id="e5d84-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e5d84-129">The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

|<span data-ttu-id="e5d84-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5d84-130">Property</span></span>|<span data-ttu-id="e5d84-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5d84-131">Type</span></span>|<span data-ttu-id="e5d84-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5d84-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5d84-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="e5d84-133">targetGroupId</span></span>|<span data-ttu-id="e5d84-134">String</span><span class="sxs-lookup"><span data-stu-id="e5d84-134">String</span></span>|<span data-ttu-id="e5d84-135">A ID do grupo do AAD no qual a configuração de provisionamento do aplicativo está sendo direcionada.</span><span class="sxs-lookup"><span data-stu-id="e5d84-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="e5d84-136">id</span><span class="sxs-lookup"><span data-stu-id="e5d84-136">id</span></span>|<span data-ttu-id="e5d84-137">String</span><span class="sxs-lookup"><span data-stu-id="e5d84-137">String</span></span>|<span data-ttu-id="e5d84-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e5d84-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="e5d84-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5d84-139">Response</span></span>
<span data-ttu-id="e5d84-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5d84-140">If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5d84-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5d84-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5d84-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5d84-142">Request</span></span>
<span data-ttu-id="e5d84-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5d84-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="e5d84-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5d84-144">Response</span></span>
<span data-ttu-id="e5d84-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5d84-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






---
title: Criar mobileAppProvisioningConfigGroupAssignment
description: Criar um novo objeto mobileAppProvisioningConfigGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c6e1584bee2de8004c343bf144dd5712e09874c5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960626"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="35c7e-103">Criar mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="35c7e-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="35c7e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="35c7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35c7e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="35c7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35c7e-106">Criar um novo objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="35c7e-106">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35c7e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="35c7e-107">Prerequisites</span></span>
<span data-ttu-id="35c7e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35c7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35c7e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35c7e-110">Permission type</span></span>|<span data-ttu-id="35c7e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="35c7e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35c7e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35c7e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35c7e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35c7e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="35c7e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35c7e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35c7e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35c7e-115">Not supported.</span></span>|
|<span data-ttu-id="35c7e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35c7e-116">Application</span></span>|<span data-ttu-id="35c7e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35c7e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35c7e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35c7e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="35c7e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35c7e-119">Request headers</span></span>
|<span data-ttu-id="35c7e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="35c7e-120">Header</span></span>|<span data-ttu-id="35c7e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="35c7e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35c7e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="35c7e-122">Authorization</span></span>|<span data-ttu-id="35c7e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35c7e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35c7e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="35c7e-124">Accept</span></span>|<span data-ttu-id="35c7e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="35c7e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35c7e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35c7e-126">Request body</span></span>
<span data-ttu-id="35c7e-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppProvisioningConfigGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="35c7e-127">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="35c7e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppProvisioningConfigGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="35c7e-128">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="35c7e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35c7e-129">Property</span></span>|<span data-ttu-id="35c7e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="35c7e-130">Type</span></span>|<span data-ttu-id="35c7e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="35c7e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35c7e-132">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="35c7e-132">targetGroupId</span></span>|<span data-ttu-id="35c7e-133">String</span><span class="sxs-lookup"><span data-stu-id="35c7e-133">String</span></span>|<span data-ttu-id="35c7e-134">A ID do grupo do AAD no qual a configuração de provisionamento do aplicativo está sendo direcionada.</span><span class="sxs-lookup"><span data-stu-id="35c7e-134">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="35c7e-135">id</span><span class="sxs-lookup"><span data-stu-id="35c7e-135">id</span></span>|<span data-ttu-id="35c7e-136">String</span><span class="sxs-lookup"><span data-stu-id="35c7e-136">String</span></span>|<span data-ttu-id="35c7e-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="35c7e-137">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="35c7e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="35c7e-138">Response</span></span>
<span data-ttu-id="35c7e-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35c7e-139">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35c7e-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35c7e-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="35c7e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35c7e-141">Request</span></span>
<span data-ttu-id="35c7e-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35c7e-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="35c7e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="35c7e-143">Response</span></span>
<span data-ttu-id="35c7e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35c7e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






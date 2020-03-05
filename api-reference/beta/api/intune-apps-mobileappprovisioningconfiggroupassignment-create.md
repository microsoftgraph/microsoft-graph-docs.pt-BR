---
title: Criar mobileAppProvisioningConfigGroupAssignment
description: Criar um novo objeto mobileAppProvisioningConfigGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6684046b6587838370ae01349a0e0cf6a962b814
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444942"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="15541-103">Criar mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="15541-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

<span data-ttu-id="15541-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="15541-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15541-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="15541-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15541-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15541-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15541-107">Criar um novo objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="15541-107">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15541-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15541-108">Prerequisites</span></span>
<span data-ttu-id="15541-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15541-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15541-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15541-111">Permission type</span></span>|<span data-ttu-id="15541-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15541-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15541-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15541-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15541-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15541-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="15541-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15541-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15541-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15541-116">Not supported.</span></span>|
|<span data-ttu-id="15541-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15541-117">Application</span></span>|<span data-ttu-id="15541-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15541-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15541-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15541-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="15541-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15541-120">Request headers</span></span>
|<span data-ttu-id="15541-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15541-121">Header</span></span>|<span data-ttu-id="15541-122">Valor</span><span class="sxs-lookup"><span data-stu-id="15541-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15541-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="15541-123">Authorization</span></span>|<span data-ttu-id="15541-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15541-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15541-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15541-125">Accept</span></span>|<span data-ttu-id="15541-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15541-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15541-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15541-127">Request body</span></span>
<span data-ttu-id="15541-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppProvisioningConfigGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="15541-128">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="15541-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppProvisioningConfigGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="15541-129">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="15541-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15541-130">Property</span></span>|<span data-ttu-id="15541-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="15541-131">Type</span></span>|<span data-ttu-id="15541-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="15541-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15541-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="15541-133">targetGroupId</span></span>|<span data-ttu-id="15541-134">String</span><span class="sxs-lookup"><span data-stu-id="15541-134">String</span></span>|<span data-ttu-id="15541-135">A ID do grupo do AAD no qual a configuração de provisionamento do aplicativo está sendo direcionada.</span><span class="sxs-lookup"><span data-stu-id="15541-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="15541-136">id</span><span class="sxs-lookup"><span data-stu-id="15541-136">id</span></span>|<span data-ttu-id="15541-137">String</span><span class="sxs-lookup"><span data-stu-id="15541-137">String</span></span>|<span data-ttu-id="15541-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="15541-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="15541-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="15541-139">Response</span></span>
<span data-ttu-id="15541-140">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15541-140">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15541-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15541-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="15541-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15541-142">Request</span></span>
<span data-ttu-id="15541-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15541-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="15541-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="15541-144">Response</span></span>
<span data-ttu-id="15541-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15541-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






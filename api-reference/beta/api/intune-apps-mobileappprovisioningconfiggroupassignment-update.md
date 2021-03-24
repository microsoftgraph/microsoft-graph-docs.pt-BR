---
title: Atualizar mobileAppProvisioningConfigGroupAssignment
description: Atualize as propriedades de um objeto mobileAppProvisioningConfigGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f783d960c9ec679e2d1644dec60561d8e55f2e6a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139637"
---
# <a name="update-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="1f930-103">Atualizar mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1f930-103">Update mobileAppProvisioningConfigGroupAssignment</span></span>

<span data-ttu-id="1f930-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f930-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f930-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1f930-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f930-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f930-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f930-107">Atualize as propriedades de [um objeto mobileAppProvisioningConfigGroupAssignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1f930-107">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f930-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1f930-108">Prerequisites</span></span>
<span data-ttu-id="1f930-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f930-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f930-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f930-111">Permission type</span></span>|<span data-ttu-id="1f930-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f930-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f930-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f930-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f930-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f930-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1f930-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f930-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f930-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f930-116">Not supported.</span></span>|
|<span data-ttu-id="1f930-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f930-117">Application</span></span>|<span data-ttu-id="1f930-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f930-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f930-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f930-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1f930-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f930-120">Request headers</span></span>
|<span data-ttu-id="1f930-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1f930-121">Header</span></span>|<span data-ttu-id="1f930-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1f930-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f930-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f930-123">Authorization</span></span>|<span data-ttu-id="1f930-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f930-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f930-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1f930-125">Accept</span></span>|<span data-ttu-id="1f930-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f930-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f930-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f930-127">Request body</span></span>
<span data-ttu-id="1f930-128">No corpo da solicitação, fornece uma representação JSON para [o objeto mobileAppProvisioningConfigGroupAssignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1f930-128">In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

<span data-ttu-id="1f930-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1f930-129">The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

|<span data-ttu-id="1f930-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f930-130">Property</span></span>|<span data-ttu-id="1f930-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f930-131">Type</span></span>|<span data-ttu-id="1f930-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f930-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f930-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="1f930-133">targetGroupId</span></span>|<span data-ttu-id="1f930-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f930-134">String</span></span>|<span data-ttu-id="1f930-135">A ID do grupo AAD no qual a configuração de provisionamento de aplicativo está sendo direcionada.</span><span class="sxs-lookup"><span data-stu-id="1f930-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="1f930-136">id</span><span class="sxs-lookup"><span data-stu-id="1f930-136">id</span></span>|<span data-ttu-id="1f930-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f930-137">String</span></span>|<span data-ttu-id="1f930-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1f930-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="1f930-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f930-139">Response</span></span>
<span data-ttu-id="1f930-140">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f930-140">If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f930-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f930-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f930-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f930-142">Request</span></span>
<span data-ttu-id="1f930-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f930-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="1f930-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f930-144">Response</span></span>
<span data-ttu-id="1f930-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f930-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





---
title: Criar mobileAppProvisioningConfigGroupAssignment
description: Crie um novo objeto mobileAppProvisioningConfigGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 173f8704ffb44750e3ef382160363dc6e1ce2e48
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139682"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="038ae-103">Criar mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="038ae-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

<span data-ttu-id="038ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="038ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="038ae-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="038ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="038ae-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="038ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="038ae-107">Crie um novo [objeto mobileAppProvisioningConfigGroupAssignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="038ae-107">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="038ae-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="038ae-108">Prerequisites</span></span>
<span data-ttu-id="038ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="038ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="038ae-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="038ae-111">Permission type</span></span>|<span data-ttu-id="038ae-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="038ae-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="038ae-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="038ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="038ae-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="038ae-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="038ae-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="038ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="038ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="038ae-116">Not supported.</span></span>|
|<span data-ttu-id="038ae-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="038ae-117">Application</span></span>|<span data-ttu-id="038ae-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="038ae-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="038ae-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="038ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="038ae-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="038ae-120">Request headers</span></span>
|<span data-ttu-id="038ae-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="038ae-121">Header</span></span>|<span data-ttu-id="038ae-122">Valor</span><span class="sxs-lookup"><span data-stu-id="038ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="038ae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="038ae-123">Authorization</span></span>|<span data-ttu-id="038ae-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="038ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="038ae-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="038ae-125">Accept</span></span>|<span data-ttu-id="038ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="038ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="038ae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="038ae-127">Request body</span></span>
<span data-ttu-id="038ae-128">No corpo da solicitação, fornece uma representação JSON para o objeto mobileAppProvisioningConfigGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="038ae-128">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="038ae-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o mobileAppProvisioningConfigGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="038ae-129">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="038ae-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="038ae-130">Property</span></span>|<span data-ttu-id="038ae-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="038ae-131">Type</span></span>|<span data-ttu-id="038ae-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="038ae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="038ae-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="038ae-133">targetGroupId</span></span>|<span data-ttu-id="038ae-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="038ae-134">String</span></span>|<span data-ttu-id="038ae-135">A ID do grupo AAD no qual a configuração de provisionamento de aplicativo está sendo direcionada.</span><span class="sxs-lookup"><span data-stu-id="038ae-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="038ae-136">id</span><span class="sxs-lookup"><span data-stu-id="038ae-136">id</span></span>|<span data-ttu-id="038ae-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="038ae-137">String</span></span>|<span data-ttu-id="038ae-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="038ae-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="038ae-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="038ae-139">Response</span></span>
<span data-ttu-id="038ae-140">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="038ae-140">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="038ae-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="038ae-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="038ae-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="038ae-142">Request</span></span>
<span data-ttu-id="038ae-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="038ae-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="038ae-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="038ae-144">Response</span></span>
<span data-ttu-id="038ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="038ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





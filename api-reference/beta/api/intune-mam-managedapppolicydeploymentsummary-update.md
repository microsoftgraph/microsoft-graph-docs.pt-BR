---
title: Atualizar managedAppPolicyDeploymentSummary
description: Atualizar as propriedades de um objeto managedAppPolicyDeploymentSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 480f2f8621e8d85b808ee2dd08306c53483fca6b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157950"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="944c5-103">Atualizar managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="944c5-103">Update managedAppPolicyDeploymentSummary</span></span>

<span data-ttu-id="944c5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="944c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="944c5-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="944c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="944c5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="944c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="944c5-107">Atualizar as propriedades de um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="944c5-107">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="944c5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="944c5-108">Prerequisites</span></span>
<span data-ttu-id="944c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="944c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="944c5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="944c5-111">Permission type</span></span>|<span data-ttu-id="944c5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="944c5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="944c5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="944c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="944c5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="944c5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="944c5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="944c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="944c5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="944c5-116">Not supported.</span></span>|
|<span data-ttu-id="944c5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="944c5-117">Application</span></span>|<span data-ttu-id="944c5-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="944c5-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="944c5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="944c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/deploymentSummary
```

## <a name="request-headers"></a><span data-ttu-id="944c5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="944c5-120">Request headers</span></span>
|<span data-ttu-id="944c5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="944c5-121">Header</span></span>|<span data-ttu-id="944c5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="944c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="944c5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="944c5-123">Authorization</span></span>|<span data-ttu-id="944c5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="944c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="944c5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="944c5-125">Accept</span></span>|<span data-ttu-id="944c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="944c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="944c5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="944c5-127">Request body</span></span>
<span data-ttu-id="944c5-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="944c5-128">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="944c5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="944c5-129">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="944c5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="944c5-130">Property</span></span>|<span data-ttu-id="944c5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="944c5-131">Type</span></span>|<span data-ttu-id="944c5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="944c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="944c5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="944c5-133">displayName</span></span>|<span data-ttu-id="944c5-134">String</span><span class="sxs-lookup"><span data-stu-id="944c5-134">String</span></span>|<span data-ttu-id="944c5-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="944c5-135">Not yet documented</span></span>|
|<span data-ttu-id="944c5-136">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="944c5-136">configurationDeployedUserCount</span></span>|<span data-ttu-id="944c5-137">Int32</span><span class="sxs-lookup"><span data-stu-id="944c5-137">Int32</span></span>|<span data-ttu-id="944c5-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="944c5-138">Not yet documented</span></span>|
|<span data-ttu-id="944c5-139">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="944c5-139">lastRefreshTime</span></span>|<span data-ttu-id="944c5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="944c5-140">DateTimeOffset</span></span>|<span data-ttu-id="944c5-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="944c5-141">Not yet documented</span></span>|
|<span data-ttu-id="944c5-142">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="944c5-142">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="944c5-143">Conjunto [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="944c5-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="944c5-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="944c5-144">Not yet documented</span></span>|
|<span data-ttu-id="944c5-145">id</span><span class="sxs-lookup"><span data-stu-id="944c5-145">id</span></span>|<span data-ttu-id="944c5-146">String</span><span class="sxs-lookup"><span data-stu-id="944c5-146">String</span></span>|<span data-ttu-id="944c5-147">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="944c5-147">Key of the entity.</span></span>|
|<span data-ttu-id="944c5-148">versão</span><span class="sxs-lookup"><span data-stu-id="944c5-148">version</span></span>|<span data-ttu-id="944c5-149">String</span><span class="sxs-lookup"><span data-stu-id="944c5-149">String</span></span>|<span data-ttu-id="944c5-150">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="944c5-150">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="944c5-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="944c5-151">Response</span></span>
<span data-ttu-id="944c5-152">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="944c5-152">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="944c5-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="944c5-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="944c5-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="944c5-154">Request</span></span>
<span data-ttu-id="944c5-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="944c5-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
Content-type: application/json
Content-length: 589

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.windowsAppIdentifier",
        "windowsAppId": "Windows App Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="944c5-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="944c5-156">Response</span></span>
<span data-ttu-id="944c5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="944c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 638

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.windowsAppIdentifier",
        "windowsAppId": "Windows App Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "id": "61f2f688-f688-61f2-88f6-f26188f6f261",
  "version": "Version value"
}
```





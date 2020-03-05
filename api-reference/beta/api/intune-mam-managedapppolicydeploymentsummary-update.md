---
title: Atualizar managedAppPolicyDeploymentSummary
description: Atualizar as propriedades de um objeto managedAppPolicyDeploymentSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b95c208cef65d23418ce06c97d8a0a68eb755a06
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463500"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="2a4cd-103">Atualizar managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="2a4cd-103">Update managedAppPolicyDeploymentSummary</span></span>

<span data-ttu-id="2a4cd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2a4cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a4cd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2a4cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a4cd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2a4cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a4cd-107">Atualizar as propriedades de um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2a4cd-107">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a4cd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2a4cd-108">Prerequisites</span></span>
<span data-ttu-id="2a4cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a4cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a4cd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a4cd-111">Permission type</span></span>|<span data-ttu-id="2a4cd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2a4cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a4cd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a4cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a4cd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a4cd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2a4cd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a4cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a4cd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a4cd-116">Not supported.</span></span>|
|<span data-ttu-id="2a4cd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a4cd-117">Application</span></span>|<span data-ttu-id="2a4cd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a4cd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a4cd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a4cd-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2a4cd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4cd-120">Request headers</span></span>
|<span data-ttu-id="2a4cd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a4cd-121">Header</span></span>|<span data-ttu-id="2a4cd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2a4cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a4cd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a4cd-123">Authorization</span></span>|<span data-ttu-id="2a4cd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a4cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a4cd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2a4cd-125">Accept</span></span>|<span data-ttu-id="2a4cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a4cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a4cd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4cd-127">Request body</span></span>
<span data-ttu-id="2a4cd-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2a4cd-128">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="2a4cd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2a4cd-129">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="2a4cd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a4cd-130">Property</span></span>|<span data-ttu-id="2a4cd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a4cd-131">Type</span></span>|<span data-ttu-id="2a4cd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a4cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a4cd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2a4cd-133">displayName</span></span>|<span data-ttu-id="2a4cd-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a4cd-134">String</span></span>|<span data-ttu-id="2a4cd-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2a4cd-135">Not yet documented</span></span>|
|<span data-ttu-id="2a4cd-136">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="2a4cd-136">configurationDeployedUserCount</span></span>|<span data-ttu-id="2a4cd-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2a4cd-137">Int32</span></span>|<span data-ttu-id="2a4cd-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2a4cd-138">Not yet documented</span></span>|
|<span data-ttu-id="2a4cd-139">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="2a4cd-139">lastRefreshTime</span></span>|<span data-ttu-id="2a4cd-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a4cd-140">DateTimeOffset</span></span>|<span data-ttu-id="2a4cd-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2a4cd-141">Not yet documented</span></span>|
|<span data-ttu-id="2a4cd-142">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="2a4cd-142">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="2a4cd-143">Conjunto [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a4cd-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="2a4cd-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2a4cd-144">Not yet documented</span></span>|
|<span data-ttu-id="2a4cd-145">id</span><span class="sxs-lookup"><span data-stu-id="2a4cd-145">id</span></span>|<span data-ttu-id="2a4cd-146">String</span><span class="sxs-lookup"><span data-stu-id="2a4cd-146">String</span></span>|<span data-ttu-id="2a4cd-147">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2a4cd-147">Key of the entity.</span></span>|
|<span data-ttu-id="2a4cd-148">versão</span><span class="sxs-lookup"><span data-stu-id="2a4cd-148">version</span></span>|<span data-ttu-id="2a4cd-149">String</span><span class="sxs-lookup"><span data-stu-id="2a4cd-149">String</span></span>|<span data-ttu-id="2a4cd-150">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="2a4cd-150">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="2a4cd-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a4cd-151">Response</span></span>
<span data-ttu-id="2a4cd-152">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a4cd-152">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a4cd-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a4cd-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a4cd-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4cd-154">Request</span></span>
<span data-ttu-id="2a4cd-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a4cd-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
Content-type: application/json
Content-length: 588

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="2a4cd-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a4cd-156">Response</span></span>
<span data-ttu-id="2a4cd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a4cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 637

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "id": "61f2f688-f688-61f2-88f6-f26188f6f261",
  "version": "Version value"
}
```






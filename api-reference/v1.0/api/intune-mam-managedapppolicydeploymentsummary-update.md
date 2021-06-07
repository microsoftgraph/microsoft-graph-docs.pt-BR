---
title: Atualizar managedAppPolicyDeploymentSummary
description: Atualizar as propriedades de um objeto managedAppPolicyDeploymentSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af97bda63cbcdf8f5373faa1f064f8f201b8ef36
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756965"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="a5f86-103">Atualizar managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="a5f86-103">Update managedAppPolicyDeploymentSummary</span></span>

<span data-ttu-id="a5f86-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5f86-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5f86-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a5f86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5f86-106">Atualizar as propriedades de um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a5f86-106">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5f86-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a5f86-107">Prerequisites</span></span>
<span data-ttu-id="a5f86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5f86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5f86-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5f86-110">Permission type</span></span>|<span data-ttu-id="a5f86-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5f86-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5f86-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5f86-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5f86-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5f86-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a5f86-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5f86-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5f86-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5f86-115">Not supported.</span></span>|
|<span data-ttu-id="a5f86-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5f86-116">Application</span></span>|<span data-ttu-id="a5f86-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5f86-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5f86-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5f86-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a5f86-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5f86-119">Request headers</span></span>
|<span data-ttu-id="a5f86-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5f86-120">Header</span></span>|<span data-ttu-id="a5f86-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a5f86-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5f86-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5f86-122">Authorization</span></span>|<span data-ttu-id="a5f86-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5f86-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5f86-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a5f86-124">Accept</span></span>|<span data-ttu-id="a5f86-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5f86-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5f86-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5f86-126">Request body</span></span>
<span data-ttu-id="a5f86-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a5f86-127">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="a5f86-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a5f86-128">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="a5f86-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5f86-129">Property</span></span>|<span data-ttu-id="a5f86-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5f86-130">Type</span></span>|<span data-ttu-id="a5f86-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5f86-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5f86-132">displayName</span><span class="sxs-lookup"><span data-stu-id="a5f86-132">displayName</span></span>|<span data-ttu-id="a5f86-133">String</span><span class="sxs-lookup"><span data-stu-id="a5f86-133">String</span></span>|<span data-ttu-id="a5f86-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a5f86-134">Not yet documented</span></span>|
|<span data-ttu-id="a5f86-135">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="a5f86-135">configurationDeployedUserCount</span></span>|<span data-ttu-id="a5f86-136">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f86-136">Int32</span></span>|<span data-ttu-id="a5f86-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a5f86-137">Not yet documented</span></span>|
|<span data-ttu-id="a5f86-138">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="a5f86-138">lastRefreshTime</span></span>|<span data-ttu-id="a5f86-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5f86-139">DateTimeOffset</span></span>|<span data-ttu-id="a5f86-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a5f86-140">Not yet documented</span></span>|
|<span data-ttu-id="a5f86-141">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="a5f86-141">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="a5f86-142">Conjunto [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="a5f86-142">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="a5f86-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a5f86-143">Not yet documented</span></span>|
|<span data-ttu-id="a5f86-144">id</span><span class="sxs-lookup"><span data-stu-id="a5f86-144">id</span></span>|<span data-ttu-id="a5f86-145">String</span><span class="sxs-lookup"><span data-stu-id="a5f86-145">String</span></span>|<span data-ttu-id="a5f86-146">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a5f86-146">Key of the entity.</span></span>|
|<span data-ttu-id="a5f86-147">versão</span><span class="sxs-lookup"><span data-stu-id="a5f86-147">version</span></span>|<span data-ttu-id="a5f86-148">String</span><span class="sxs-lookup"><span data-stu-id="a5f86-148">String</span></span>|<span data-ttu-id="a5f86-149">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="a5f86-149">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="a5f86-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5f86-150">Response</span></span>
<span data-ttu-id="a5f86-151">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5f86-151">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5f86-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5f86-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5f86-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5f86-153">Request</span></span>
<span data-ttu-id="a5f86-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5f86-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
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

### <a name="response"></a><span data-ttu-id="a5f86-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5f86-155">Response</span></span>
<span data-ttu-id="a5f86-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5f86-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





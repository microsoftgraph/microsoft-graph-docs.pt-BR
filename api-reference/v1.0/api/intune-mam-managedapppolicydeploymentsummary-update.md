---
title: Atualizar managedAppPolicyDeploymentSummary
description: Atualizar as propriedades de um objeto managedAppPolicyDeploymentSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: feb753b0c881a3d5e4a91f181eba9174d1765020
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018229"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="b8709-103">Atualizar managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="b8709-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="b8709-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8709-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8709-105">Atualizar as propriedades de um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b8709-105">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8709-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8709-106">Prerequisites</span></span>
<span data-ttu-id="b8709-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8709-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8709-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8709-109">Permission type</span></span>|<span data-ttu-id="b8709-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b8709-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8709-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8709-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8709-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8709-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b8709-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8709-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8709-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8709-114">Not supported.</span></span>|
|<span data-ttu-id="b8709-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8709-115">Application</span></span>|<span data-ttu-id="b8709-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8709-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8709-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8709-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b8709-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8709-118">Request headers</span></span>
|<span data-ttu-id="b8709-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8709-119">Header</span></span>|<span data-ttu-id="b8709-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b8709-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8709-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8709-121">Authorization</span></span>|<span data-ttu-id="b8709-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8709-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8709-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b8709-123">Accept</span></span>|<span data-ttu-id="b8709-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b8709-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8709-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8709-125">Request body</span></span>
<span data-ttu-id="b8709-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b8709-126">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="b8709-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b8709-127">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="b8709-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8709-128">Property</span></span>|<span data-ttu-id="b8709-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8709-129">Type</span></span>|<span data-ttu-id="b8709-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8709-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8709-131">displayName</span><span class="sxs-lookup"><span data-stu-id="b8709-131">displayName</span></span>|<span data-ttu-id="b8709-132">String</span><span class="sxs-lookup"><span data-stu-id="b8709-132">String</span></span>|<span data-ttu-id="b8709-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b8709-133">Not yet documented</span></span>|
|<span data-ttu-id="b8709-134">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="b8709-134">configurationDeployedUserCount</span></span>|<span data-ttu-id="b8709-135">Int32</span><span class="sxs-lookup"><span data-stu-id="b8709-135">Int32</span></span>|<span data-ttu-id="b8709-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b8709-136">Not yet documented</span></span>|
|<span data-ttu-id="b8709-137">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="b8709-137">lastRefreshTime</span></span>|<span data-ttu-id="b8709-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8709-138">DateTimeOffset</span></span>|<span data-ttu-id="b8709-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b8709-139">Not yet documented</span></span>|
|<span data-ttu-id="b8709-140">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="b8709-140">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="b8709-141">Conjunto [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="b8709-141">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="b8709-142">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b8709-142">Not yet documented</span></span>|
|<span data-ttu-id="b8709-143">id</span><span class="sxs-lookup"><span data-stu-id="b8709-143">id</span></span>|<span data-ttu-id="b8709-144">String</span><span class="sxs-lookup"><span data-stu-id="b8709-144">String</span></span>|<span data-ttu-id="b8709-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b8709-145">Key of the entity.</span></span>|
|<span data-ttu-id="b8709-146">versão</span><span class="sxs-lookup"><span data-stu-id="b8709-146">version</span></span>|<span data-ttu-id="b8709-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8709-147">String</span></span>|<span data-ttu-id="b8709-148">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="b8709-148">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b8709-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8709-149">Response</span></span>
<span data-ttu-id="b8709-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8709-150">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8709-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8709-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8709-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8709-152">Request</span></span>
<span data-ttu-id="b8709-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8709-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b8709-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8709-154">Response</span></span>
<span data-ttu-id="b8709-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8709-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




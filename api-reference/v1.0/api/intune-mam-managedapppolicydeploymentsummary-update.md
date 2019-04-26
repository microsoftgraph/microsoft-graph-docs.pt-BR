---
title: Atualizar managedAppPolicyDeploymentSummary
description: Atualizar as propriedades de um objeto managedAppPolicyDeploymentSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63492e80bedc6a9e785f572e01db7c07b4cde8a7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570929"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="0f0bb-103">Atualizar managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="0f0bb-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="0f0bb-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f0bb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f0bb-105">Atualizar as propriedades de um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="0f0bb-105">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f0bb-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f0bb-106">Prerequisites</span></span>
<span data-ttu-id="0f0bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f0bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f0bb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f0bb-109">Permission type</span></span>|<span data-ttu-id="0f0bb-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0f0bb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f0bb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f0bb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0f0bb-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f0bb-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0f0bb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f0bb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f0bb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f0bb-114">Not supported.</span></span>|
|<span data-ttu-id="0f0bb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f0bb-115">Application</span></span>|<span data-ttu-id="0f0bb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f0bb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f0bb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f0bb-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0f0bb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f0bb-118">Request headers</span></span>
|<span data-ttu-id="0f0bb-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f0bb-119">Header</span></span>|<span data-ttu-id="0f0bb-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0f0bb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f0bb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f0bb-121">Authorization</span></span>|<span data-ttu-id="0f0bb-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f0bb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f0bb-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0f0bb-123">Accept</span></span>|<span data-ttu-id="0f0bb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0f0bb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f0bb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f0bb-125">Request body</span></span>
<span data-ttu-id="0f0bb-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="0f0bb-126">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="0f0bb-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="0f0bb-127">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="0f0bb-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f0bb-128">Property</span></span>|<span data-ttu-id="0f0bb-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f0bb-129">Type</span></span>|<span data-ttu-id="0f0bb-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f0bb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f0bb-131">displayName</span><span class="sxs-lookup"><span data-stu-id="0f0bb-131">displayName</span></span>|<span data-ttu-id="0f0bb-132">String</span><span class="sxs-lookup"><span data-stu-id="0f0bb-132">String</span></span>|<span data-ttu-id="0f0bb-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0f0bb-133">Not yet documented</span></span>|
|<span data-ttu-id="0f0bb-134">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="0f0bb-134">configurationDeployedUserCount</span></span>|<span data-ttu-id="0f0bb-135">Int32</span><span class="sxs-lookup"><span data-stu-id="0f0bb-135">Int32</span></span>|<span data-ttu-id="0f0bb-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0f0bb-136">Not yet documented</span></span>|
|<span data-ttu-id="0f0bb-137">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="0f0bb-137">lastRefreshTime</span></span>|<span data-ttu-id="0f0bb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f0bb-138">DateTimeOffset</span></span>|<span data-ttu-id="0f0bb-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0f0bb-139">Not yet documented</span></span>|
|<span data-ttu-id="0f0bb-140">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="0f0bb-140">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="0f0bb-141">Conjunto [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f0bb-141">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="0f0bb-142">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0f0bb-142">Not yet documented</span></span>|
|<span data-ttu-id="0f0bb-143">id</span><span class="sxs-lookup"><span data-stu-id="0f0bb-143">id</span></span>|<span data-ttu-id="0f0bb-144">String</span><span class="sxs-lookup"><span data-stu-id="0f0bb-144">String</span></span>|<span data-ttu-id="0f0bb-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0f0bb-145">Key of the entity.</span></span>|
|<span data-ttu-id="0f0bb-146">versão</span><span class="sxs-lookup"><span data-stu-id="0f0bb-146">version</span></span>|<span data-ttu-id="0f0bb-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f0bb-147">String</span></span>|<span data-ttu-id="0f0bb-148">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="0f0bb-148">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="0f0bb-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f0bb-149">Response</span></span>
<span data-ttu-id="0f0bb-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f0bb-150">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f0bb-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f0bb-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f0bb-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f0bb-152">Request</span></span>
<span data-ttu-id="0f0bb-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f0bb-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0f0bb-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f0bb-154">Response</span></span>
<span data-ttu-id="0f0bb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f0bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




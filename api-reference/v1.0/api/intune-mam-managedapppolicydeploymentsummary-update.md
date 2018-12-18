---
title: Atualizar managedAppPolicyDeploymentSummary
description: Atualizar as propriedades de um objeto managedAppPolicyDeploymentSummary.
author: tfitzmac
ms.openlocfilehash: e123c07722e9bd4baf2cab7bfd5f53516b37a949
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342956"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="a1a33-103">Atualizar managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="a1a33-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="a1a33-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a1a33-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1a33-105">Atualizar as propriedades de um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a1a33-105">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1a33-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1a33-106">Prerequisites</span></span>
<span data-ttu-id="a1a33-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1a33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1a33-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1a33-109">Permission type</span></span>|<span data-ttu-id="a1a33-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1a33-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1a33-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1a33-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a1a33-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1a33-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a1a33-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1a33-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1a33-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1a33-114">Not supported.</span></span>|
|<span data-ttu-id="a1a33-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1a33-115">Application</span></span>|<span data-ttu-id="a1a33-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1a33-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1a33-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1a33-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a1a33-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1a33-118">Request headers</span></span>
|<span data-ttu-id="a1a33-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1a33-119">Header</span></span>|<span data-ttu-id="a1a33-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a1a33-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1a33-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1a33-121">Authorization</span></span>|<span data-ttu-id="a1a33-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1a33-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1a33-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a1a33-123">Accept</span></span>|<span data-ttu-id="a1a33-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a1a33-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1a33-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1a33-125">Request body</span></span>
<span data-ttu-id="a1a33-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a1a33-126">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="a1a33-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a1a33-127">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="a1a33-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1a33-128">Property</span></span>|<span data-ttu-id="a1a33-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1a33-129">Type</span></span>|<span data-ttu-id="a1a33-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1a33-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1a33-131">displayName</span><span class="sxs-lookup"><span data-stu-id="a1a33-131">displayName</span></span>|<span data-ttu-id="a1a33-132">String</span><span class="sxs-lookup"><span data-stu-id="a1a33-132">String</span></span>|<span data-ttu-id="a1a33-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1a33-133">Not yet documented</span></span>|
|<span data-ttu-id="a1a33-134">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="a1a33-134">configurationDeployedUserCount</span></span>|<span data-ttu-id="a1a33-135">Int32</span><span class="sxs-lookup"><span data-stu-id="a1a33-135">Int32</span></span>|<span data-ttu-id="a1a33-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1a33-136">Not yet documented</span></span>|
|<span data-ttu-id="a1a33-137">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="a1a33-137">lastRefreshTime</span></span>|<span data-ttu-id="a1a33-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1a33-138">DateTimeOffset</span></span>|<span data-ttu-id="a1a33-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1a33-139">Not yet documented</span></span>|
|<span data-ttu-id="a1a33-140">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="a1a33-140">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="a1a33-141">Conjunto [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1a33-141">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="a1a33-142">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1a33-142">Not yet documented</span></span>|
|<span data-ttu-id="a1a33-143">id</span><span class="sxs-lookup"><span data-stu-id="a1a33-143">id</span></span>|<span data-ttu-id="a1a33-144">String</span><span class="sxs-lookup"><span data-stu-id="a1a33-144">String</span></span>|<span data-ttu-id="a1a33-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a1a33-145">Key of the entity.</span></span>|
|<span data-ttu-id="a1a33-146">version</span><span class="sxs-lookup"><span data-stu-id="a1a33-146">version</span></span>|<span data-ttu-id="a1a33-147">String</span><span class="sxs-lookup"><span data-stu-id="a1a33-147">String</span></span>|<span data-ttu-id="a1a33-148">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="a1a33-148">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="a1a33-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1a33-149">Response</span></span>
<span data-ttu-id="a1a33-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1a33-150">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1a33-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1a33-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1a33-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1a33-152">Request</span></span>
<span data-ttu-id="a1a33-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1a33-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a1a33-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1a33-154">Response</span></span>
<span data-ttu-id="a1a33-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1a33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




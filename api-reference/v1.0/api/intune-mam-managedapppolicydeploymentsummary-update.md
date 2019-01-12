---
title: Atualizar managedAppPolicyDeploymentSummary
description: Atualizar as propriedades de um objeto managedAppPolicyDeploymentSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b8282d48fc6dc109857a0ff9bac037612cb54d93
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929071"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="0fc61-103">Atualizar managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="0fc61-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="0fc61-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0fc61-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0fc61-105">Atualizar as propriedades de um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="0fc61-105">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0fc61-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0fc61-106">Prerequisites</span></span>
<span data-ttu-id="0fc61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fc61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fc61-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fc61-109">Permission type</span></span>|<span data-ttu-id="0fc61-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0fc61-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fc61-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fc61-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0fc61-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fc61-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0fc61-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fc61-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fc61-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fc61-114">Not supported.</span></span>|
|<span data-ttu-id="0fc61-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fc61-115">Application</span></span>|<span data-ttu-id="0fc61-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fc61-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fc61-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fc61-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0fc61-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fc61-118">Request headers</span></span>
|<span data-ttu-id="0fc61-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0fc61-119">Header</span></span>|<span data-ttu-id="0fc61-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0fc61-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fc61-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fc61-121">Authorization</span></span>|<span data-ttu-id="0fc61-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fc61-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fc61-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0fc61-123">Accept</span></span>|<span data-ttu-id="0fc61-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0fc61-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fc61-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fc61-125">Request body</span></span>
<span data-ttu-id="0fc61-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="0fc61-126">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="0fc61-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="0fc61-127">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="0fc61-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0fc61-128">Property</span></span>|<span data-ttu-id="0fc61-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0fc61-129">Type</span></span>|<span data-ttu-id="0fc61-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fc61-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fc61-131">displayName</span><span class="sxs-lookup"><span data-stu-id="0fc61-131">displayName</span></span>|<span data-ttu-id="0fc61-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0fc61-132">String</span></span>|<span data-ttu-id="0fc61-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0fc61-133">Not yet documented</span></span>|
|<span data-ttu-id="0fc61-134">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="0fc61-134">configurationDeployedUserCount</span></span>|<span data-ttu-id="0fc61-135">Int32</span><span class="sxs-lookup"><span data-stu-id="0fc61-135">Int32</span></span>|<span data-ttu-id="0fc61-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0fc61-136">Not yet documented</span></span>|
|<span data-ttu-id="0fc61-137">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="0fc61-137">lastRefreshTime</span></span>|<span data-ttu-id="0fc61-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fc61-138">DateTimeOffset</span></span>|<span data-ttu-id="0fc61-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0fc61-139">Not yet documented</span></span>|
|<span data-ttu-id="0fc61-140">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="0fc61-140">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="0fc61-141">Conjunto [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fc61-141">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="0fc61-142">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0fc61-142">Not yet documented</span></span>|
|<span data-ttu-id="0fc61-143">id</span><span class="sxs-lookup"><span data-stu-id="0fc61-143">id</span></span>|<span data-ttu-id="0fc61-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0fc61-144">String</span></span>|<span data-ttu-id="0fc61-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0fc61-145">Key of the entity.</span></span>|
|<span data-ttu-id="0fc61-146">version</span><span class="sxs-lookup"><span data-stu-id="0fc61-146">version</span></span>|<span data-ttu-id="0fc61-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0fc61-147">String</span></span>|<span data-ttu-id="0fc61-148">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="0fc61-148">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="0fc61-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fc61-149">Response</span></span>
<span data-ttu-id="0fc61-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fc61-150">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fc61-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fc61-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="0fc61-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fc61-152">Request</span></span>
<span data-ttu-id="0fc61-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fc61-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0fc61-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fc61-154">Response</span></span>
<span data-ttu-id="0fc61-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fc61-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




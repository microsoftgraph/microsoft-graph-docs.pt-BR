---
title: Atualizar managedAppPolicyDeploymentSummary
description: Atualizar as propriedades de um objeto managedAppPolicyDeploymentSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 220443e5c75121083fb23758e42d7ec331bbee18
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877418"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="11f1f-103">Atualizar managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="11f1f-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="11f1f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="11f1f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11f1f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="11f1f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11f1f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="11f1f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11f1f-107">Atualizar as propriedades de um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="11f1f-107">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="11f1f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="11f1f-108">Prerequisites</span></span>
<span data-ttu-id="11f1f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11f1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11f1f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11f1f-111">Permission type</span></span>|<span data-ttu-id="11f1f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="11f1f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11f1f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11f1f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11f1f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11f1f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="11f1f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11f1f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11f1f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11f1f-116">Not supported.</span></span>|
|<span data-ttu-id="11f1f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11f1f-117">Application</span></span>|<span data-ttu-id="11f1f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11f1f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11f1f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11f1f-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="11f1f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11f1f-120">Request headers</span></span>
|<span data-ttu-id="11f1f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11f1f-121">Header</span></span>|<span data-ttu-id="11f1f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="11f1f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11f1f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="11f1f-123">Authorization</span></span>|<span data-ttu-id="11f1f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11f1f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11f1f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="11f1f-125">Accept</span></span>|<span data-ttu-id="11f1f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11f1f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11f1f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11f1f-127">Request body</span></span>
<span data-ttu-id="11f1f-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="11f1f-128">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="11f1f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="11f1f-129">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="11f1f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11f1f-130">Property</span></span>|<span data-ttu-id="11f1f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="11f1f-131">Type</span></span>|<span data-ttu-id="11f1f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="11f1f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11f1f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="11f1f-133">displayName</span></span>|<span data-ttu-id="11f1f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11f1f-134">String</span></span>|<span data-ttu-id="11f1f-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="11f1f-135">Not yet documented</span></span>|
|<span data-ttu-id="11f1f-136">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="11f1f-136">configurationDeployedUserCount</span></span>|<span data-ttu-id="11f1f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="11f1f-137">Int32</span></span>|<span data-ttu-id="11f1f-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="11f1f-138">Not yet documented</span></span>|
|<span data-ttu-id="11f1f-139">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="11f1f-139">lastRefreshTime</span></span>|<span data-ttu-id="11f1f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11f1f-140">DateTimeOffset</span></span>|<span data-ttu-id="11f1f-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="11f1f-141">Not yet documented</span></span>|
|<span data-ttu-id="11f1f-142">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="11f1f-142">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="11f1f-143">Conjunto [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="11f1f-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="11f1f-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="11f1f-144">Not yet documented</span></span>|
|<span data-ttu-id="11f1f-145">id</span><span class="sxs-lookup"><span data-stu-id="11f1f-145">id</span></span>|<span data-ttu-id="11f1f-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11f1f-146">String</span></span>|<span data-ttu-id="11f1f-147">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="11f1f-147">Key of the entity.</span></span>|
|<span data-ttu-id="11f1f-148">version</span><span class="sxs-lookup"><span data-stu-id="11f1f-148">version</span></span>|<span data-ttu-id="11f1f-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11f1f-149">String</span></span>|<span data-ttu-id="11f1f-150">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="11f1f-150">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="11f1f-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="11f1f-151">Response</span></span>
<span data-ttu-id="11f1f-152">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11f1f-152">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11f1f-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11f1f-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="11f1f-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11f1f-154">Request</span></span>
<span data-ttu-id="11f1f-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11f1f-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
Content-type: application/json
Content-length: 516

{
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

### <a name="response"></a><span data-ttu-id="11f1f-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="11f1f-156">Response</span></span>
<span data-ttu-id="11f1f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11f1f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






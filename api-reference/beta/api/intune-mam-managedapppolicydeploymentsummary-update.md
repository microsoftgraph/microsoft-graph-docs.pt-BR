---
title: Atualizar managedAppPolicyDeploymentSummary
description: Atualizar as propriedades de um objeto managedAppPolicyDeploymentSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f940bac34deca1aa938784eee514b765a78ce64a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408142"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="c1d7c-103">Atualizar managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="c1d7c-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="c1d7c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c1d7c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c1d7c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c1d7c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1d7c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c1d7c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1d7c-107">Atualizar as propriedades de um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c1d7c-107">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1d7c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c1d7c-108">Prerequisites</span></span>
<span data-ttu-id="c1d7c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c1d7c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c1d7c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1d7c-111">Permission type</span></span>|<span data-ttu-id="c1d7c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c1d7c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1d7c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1d7c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1d7c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1d7c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c1d7c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1d7c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1d7c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1d7c-116">Not supported.</span></span>|
|<span data-ttu-id="c1d7c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1d7c-117">Application</span></span>|<span data-ttu-id="c1d7c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1d7c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1d7c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1d7c-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c1d7c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1d7c-120">Request headers</span></span>
|<span data-ttu-id="c1d7c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c1d7c-121">Header</span></span>|<span data-ttu-id="c1d7c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c1d7c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1d7c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1d7c-123">Authorization</span></span>|<span data-ttu-id="c1d7c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1d7c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1d7c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c1d7c-125">Accept</span></span>|<span data-ttu-id="c1d7c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1d7c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1d7c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1d7c-127">Request body</span></span>
<span data-ttu-id="c1d7c-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c1d7c-128">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="c1d7c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c1d7c-129">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="c1d7c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1d7c-130">Property</span></span>|<span data-ttu-id="c1d7c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1d7c-131">Type</span></span>|<span data-ttu-id="c1d7c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1d7c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1d7c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c1d7c-133">displayName</span></span>|<span data-ttu-id="c1d7c-134">String</span><span class="sxs-lookup"><span data-stu-id="c1d7c-134">String</span></span>|<span data-ttu-id="c1d7c-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c1d7c-135">Not yet documented</span></span>|
|<span data-ttu-id="c1d7c-136">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="c1d7c-136">configurationDeployedUserCount</span></span>|<span data-ttu-id="c1d7c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c1d7c-137">Int32</span></span>|<span data-ttu-id="c1d7c-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c1d7c-138">Not yet documented</span></span>|
|<span data-ttu-id="c1d7c-139">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="c1d7c-139">lastRefreshTime</span></span>|<span data-ttu-id="c1d7c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1d7c-140">DateTimeOffset</span></span>|<span data-ttu-id="c1d7c-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c1d7c-141">Not yet documented</span></span>|
|<span data-ttu-id="c1d7c-142">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="c1d7c-142">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="c1d7c-143">Conjunto [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1d7c-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="c1d7c-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c1d7c-144">Not yet documented</span></span>|
|<span data-ttu-id="c1d7c-145">id</span><span class="sxs-lookup"><span data-stu-id="c1d7c-145">id</span></span>|<span data-ttu-id="c1d7c-146">String</span><span class="sxs-lookup"><span data-stu-id="c1d7c-146">String</span></span>|<span data-ttu-id="c1d7c-147">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c1d7c-147">Key of the entity.</span></span>|
|<span data-ttu-id="c1d7c-148">version</span><span class="sxs-lookup"><span data-stu-id="c1d7c-148">version</span></span>|<span data-ttu-id="c1d7c-149">String</span><span class="sxs-lookup"><span data-stu-id="c1d7c-149">String</span></span>|<span data-ttu-id="c1d7c-150">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="c1d7c-150">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="c1d7c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1d7c-151">Response</span></span>
<span data-ttu-id="c1d7c-152">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1d7c-152">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1d7c-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1d7c-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1d7c-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1d7c-154">Request</span></span>
<span data-ttu-id="c1d7c-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1d7c-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1d7c-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1d7c-156">Response</span></span>
<span data-ttu-id="c1d7c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1d7c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





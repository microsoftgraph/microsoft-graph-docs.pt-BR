---
title: Atualizar managedDeviceMobileAppConfigurationDeviceSummary
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationDeviceSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9bd35add678c40a7f79e42994b0cf1c512d3d979
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329765"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="d6d9a-103">Atualizar managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="d6d9a-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="d6d9a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6d9a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6d9a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6d9a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6d9a-106">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d6d9a-106">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6d9a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6d9a-107">Prerequisites</span></span>
<span data-ttu-id="d6d9a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6d9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6d9a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6d9a-110">Permission type</span></span>|<span data-ttu-id="d6d9a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6d9a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6d9a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6d9a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6d9a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6d9a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d6d9a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6d9a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6d9a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6d9a-115">Not supported.</span></span>|
|<span data-ttu-id="d6d9a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6d9a-116">Application</span></span>|<span data-ttu-id="d6d9a-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6d9a-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6d9a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6d9a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="d6d9a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6d9a-119">Request headers</span></span>
|<span data-ttu-id="d6d9a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6d9a-120">Header</span></span>|<span data-ttu-id="d6d9a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d6d9a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6d9a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6d9a-122">Authorization</span></span>|<span data-ttu-id="d6d9a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6d9a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6d9a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6d9a-124">Accept</span></span>|<span data-ttu-id="d6d9a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d6d9a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6d9a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6d9a-126">Request body</span></span>
<span data-ttu-id="d6d9a-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d6d9a-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="d6d9a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d6d9a-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="d6d9a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6d9a-129">Property</span></span>|<span data-ttu-id="d6d9a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6d9a-130">Type</span></span>|<span data-ttu-id="d6d9a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6d9a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6d9a-132">id</span><span class="sxs-lookup"><span data-stu-id="d6d9a-132">id</span></span>|<span data-ttu-id="d6d9a-133">String</span><span class="sxs-lookup"><span data-stu-id="d6d9a-133">String</span></span>|<span data-ttu-id="d6d9a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d6d9a-134">Key of the entity.</span></span>|
|<span data-ttu-id="d6d9a-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="d6d9a-135">pendingCount</span></span>|<span data-ttu-id="d6d9a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d6d9a-136">Int32</span></span>|<span data-ttu-id="d6d9a-137">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="d6d9a-137">Number of pending devices</span></span>|
|<span data-ttu-id="d6d9a-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d6d9a-138">notApplicableCount</span></span>|<span data-ttu-id="d6d9a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d6d9a-139">Int32</span></span>|<span data-ttu-id="d6d9a-140">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="d6d9a-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="d6d9a-141">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="d6d9a-141">notApplicablePlatformCount</span></span>|<span data-ttu-id="d6d9a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d6d9a-142">Int32</span></span>|<span data-ttu-id="d6d9a-143">Número de dispositivos não aplicáveis devido à plataforma e à política incompatíveis</span><span class="sxs-lookup"><span data-stu-id="d6d9a-143">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="d6d9a-144">successCount</span><span class="sxs-lookup"><span data-stu-id="d6d9a-144">successCount</span></span>|<span data-ttu-id="d6d9a-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d6d9a-145">Int32</span></span>|<span data-ttu-id="d6d9a-146">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="d6d9a-146">Number of succeeded devices</span></span>|
|<span data-ttu-id="d6d9a-147">errorCount</span><span class="sxs-lookup"><span data-stu-id="d6d9a-147">errorCount</span></span>|<span data-ttu-id="d6d9a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d6d9a-148">Int32</span></span>|<span data-ttu-id="d6d9a-149">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="d6d9a-149">Number of error devices</span></span>|
|<span data-ttu-id="d6d9a-150">failedCount</span><span class="sxs-lookup"><span data-stu-id="d6d9a-150">failedCount</span></span>|<span data-ttu-id="d6d9a-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d6d9a-151">Int32</span></span>|<span data-ttu-id="d6d9a-152">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="d6d9a-152">Number of failed devices</span></span>|
|<span data-ttu-id="d6d9a-153">conflictCount</span><span class="sxs-lookup"><span data-stu-id="d6d9a-153">conflictCount</span></span>|<span data-ttu-id="d6d9a-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d6d9a-154">Int32</span></span>|<span data-ttu-id="d6d9a-155">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="d6d9a-155">Number of devices in conflict</span></span>|
|<span data-ttu-id="d6d9a-156">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="d6d9a-156">lastUpdateDateTime</span></span>|<span data-ttu-id="d6d9a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6d9a-157">DateTimeOffset</span></span>|<span data-ttu-id="d6d9a-158">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="d6d9a-158">Last update time</span></span>|
|<span data-ttu-id="d6d9a-159">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="d6d9a-159">configurationVersion</span></span>|<span data-ttu-id="d6d9a-160">Int32</span><span class="sxs-lookup"><span data-stu-id="d6d9a-160">Int32</span></span>|<span data-ttu-id="d6d9a-161">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="d6d9a-161">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="d6d9a-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6d9a-162">Response</span></span>
<span data-ttu-id="d6d9a-163">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6d9a-163">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6d9a-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6d9a-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6d9a-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6d9a-165">Request</span></span>
<span data-ttu-id="d6d9a-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6d9a-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="d6d9a-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6d9a-167">Response</span></span>
<span data-ttu-id="d6d9a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6d9a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "9997c455-c455-9997-55c4-979955c49799",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```







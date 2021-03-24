---
title: Atualizar managedDeviceMobileAppConfigurationDeviceSummary
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0fa4fd489e8ec5ee05aa4838c0fb84f436a902c7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143574"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="ca2f6-103">Atualizar managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="ca2f6-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

<span data-ttu-id="ca2f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca2f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca2f6-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca2f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca2f6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca2f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca2f6-107">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ca2f6-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca2f6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca2f6-108">Prerequisites</span></span>
<span data-ttu-id="ca2f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca2f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca2f6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca2f6-111">Permission type</span></span>|<span data-ttu-id="ca2f6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca2f6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca2f6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca2f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca2f6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca2f6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ca2f6-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca2f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca2f6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca2f6-116">Not supported.</span></span>|
|<span data-ttu-id="ca2f6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca2f6-117">Application</span></span>|<span data-ttu-id="ca2f6-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca2f6-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca2f6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca2f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="ca2f6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca2f6-120">Request headers</span></span>
|<span data-ttu-id="ca2f6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca2f6-121">Header</span></span>|<span data-ttu-id="ca2f6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ca2f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca2f6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca2f6-123">Authorization</span></span>|<span data-ttu-id="ca2f6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca2f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca2f6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca2f6-125">Accept</span></span>|<span data-ttu-id="ca2f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca2f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca2f6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca2f6-127">Request body</span></span>
<span data-ttu-id="ca2f6-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ca2f6-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="ca2f6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ca2f6-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="ca2f6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca2f6-130">Property</span></span>|<span data-ttu-id="ca2f6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca2f6-131">Type</span></span>|<span data-ttu-id="ca2f6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca2f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca2f6-133">id</span><span class="sxs-lookup"><span data-stu-id="ca2f6-133">id</span></span>|<span data-ttu-id="ca2f6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca2f6-134">String</span></span>|<span data-ttu-id="ca2f6-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ca2f6-135">Key of the entity.</span></span>|
|<span data-ttu-id="ca2f6-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="ca2f6-136">pendingCount</span></span>|<span data-ttu-id="ca2f6-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ca2f6-137">Int32</span></span>|<span data-ttu-id="ca2f6-138">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="ca2f6-138">Number of pending devices</span></span>|
|<span data-ttu-id="ca2f6-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="ca2f6-139">notApplicableCount</span></span>|<span data-ttu-id="ca2f6-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ca2f6-140">Int32</span></span>|<span data-ttu-id="ca2f6-141">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="ca2f6-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="ca2f6-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="ca2f6-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="ca2f6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ca2f6-143">Int32</span></span>|<span data-ttu-id="ca2f6-144">Número de dispositivos não aplicáveis devido à plataforma e à política de incompatibilidade</span><span class="sxs-lookup"><span data-stu-id="ca2f6-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="ca2f6-145">successCount</span><span class="sxs-lookup"><span data-stu-id="ca2f6-145">successCount</span></span>|<span data-ttu-id="ca2f6-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ca2f6-146">Int32</span></span>|<span data-ttu-id="ca2f6-147">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="ca2f6-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="ca2f6-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="ca2f6-148">errorCount</span></span>|<span data-ttu-id="ca2f6-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ca2f6-149">Int32</span></span>|<span data-ttu-id="ca2f6-150">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="ca2f6-150">Number of error devices</span></span>|
|<span data-ttu-id="ca2f6-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="ca2f6-151">failedCount</span></span>|<span data-ttu-id="ca2f6-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ca2f6-152">Int32</span></span>|<span data-ttu-id="ca2f6-153">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="ca2f6-153">Number of failed devices</span></span>|
|<span data-ttu-id="ca2f6-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="ca2f6-154">conflictCount</span></span>|<span data-ttu-id="ca2f6-155">Int32</span><span class="sxs-lookup"><span data-stu-id="ca2f6-155">Int32</span></span>|<span data-ttu-id="ca2f6-156">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="ca2f6-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="ca2f6-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="ca2f6-157">lastUpdateDateTime</span></span>|<span data-ttu-id="ca2f6-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca2f6-158">DateTimeOffset</span></span>|<span data-ttu-id="ca2f6-159">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="ca2f6-159">Last update time</span></span>|
|<span data-ttu-id="ca2f6-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="ca2f6-160">configurationVersion</span></span>|<span data-ttu-id="ca2f6-161">Int32</span><span class="sxs-lookup"><span data-stu-id="ca2f6-161">Int32</span></span>|<span data-ttu-id="ca2f6-162">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="ca2f6-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="ca2f6-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca2f6-163">Response</span></span>
<span data-ttu-id="ca2f6-164">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca2f6-164">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca2f6-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca2f6-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca2f6-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca2f6-166">Request</span></span>
<span data-ttu-id="ca2f6-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca2f6-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ca2f6-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca2f6-168">Response</span></span>
<span data-ttu-id="ca2f6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca2f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





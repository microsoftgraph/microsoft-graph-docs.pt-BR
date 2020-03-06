---
title: Atualizar managedDeviceMobileAppConfigurationDeviceSummary
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationDeviceSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 98a38fd33d220943aaff32bea1cca963665bb186
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516255"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="90239-103">Atualizar managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="90239-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

<span data-ttu-id="90239-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90239-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90239-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90239-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90239-106">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="90239-106">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90239-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90239-107">Prerequisites</span></span>
<span data-ttu-id="90239-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90239-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90239-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90239-110">Permission type</span></span>|<span data-ttu-id="90239-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90239-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90239-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90239-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90239-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90239-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="90239-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90239-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90239-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90239-115">Not supported.</span></span>|
|<span data-ttu-id="90239-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90239-116">Application</span></span>|<span data-ttu-id="90239-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90239-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90239-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90239-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="90239-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90239-119">Request headers</span></span>
|<span data-ttu-id="90239-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90239-120">Header</span></span>|<span data-ttu-id="90239-121">Valor</span><span class="sxs-lookup"><span data-stu-id="90239-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90239-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="90239-122">Authorization</span></span>|<span data-ttu-id="90239-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90239-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90239-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90239-124">Accept</span></span>|<span data-ttu-id="90239-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90239-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90239-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90239-126">Request body</span></span>
<span data-ttu-id="90239-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="90239-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="90239-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="90239-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="90239-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90239-129">Property</span></span>|<span data-ttu-id="90239-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="90239-130">Type</span></span>|<span data-ttu-id="90239-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="90239-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90239-132">id</span><span class="sxs-lookup"><span data-stu-id="90239-132">id</span></span>|<span data-ttu-id="90239-133">String</span><span class="sxs-lookup"><span data-stu-id="90239-133">String</span></span>|<span data-ttu-id="90239-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="90239-134">Key of the entity.</span></span>|
|<span data-ttu-id="90239-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="90239-135">pendingCount</span></span>|<span data-ttu-id="90239-136">Int32</span><span class="sxs-lookup"><span data-stu-id="90239-136">Int32</span></span>|<span data-ttu-id="90239-137">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="90239-137">Number of pending devices</span></span>|
|<span data-ttu-id="90239-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="90239-138">notApplicableCount</span></span>|<span data-ttu-id="90239-139">Int32</span><span class="sxs-lookup"><span data-stu-id="90239-139">Int32</span></span>|<span data-ttu-id="90239-140">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="90239-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="90239-141">successCount</span><span class="sxs-lookup"><span data-stu-id="90239-141">successCount</span></span>|<span data-ttu-id="90239-142">Int32</span><span class="sxs-lookup"><span data-stu-id="90239-142">Int32</span></span>|<span data-ttu-id="90239-143">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="90239-143">Number of succeeded devices</span></span>|
|<span data-ttu-id="90239-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="90239-144">errorCount</span></span>|<span data-ttu-id="90239-145">Int32</span><span class="sxs-lookup"><span data-stu-id="90239-145">Int32</span></span>|<span data-ttu-id="90239-146">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="90239-146">Number of error devices</span></span>|
|<span data-ttu-id="90239-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="90239-147">failedCount</span></span>|<span data-ttu-id="90239-148">Int32</span><span class="sxs-lookup"><span data-stu-id="90239-148">Int32</span></span>|<span data-ttu-id="90239-149">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="90239-149">Number of failed devices</span></span>|
|<span data-ttu-id="90239-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="90239-150">lastUpdateDateTime</span></span>|<span data-ttu-id="90239-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90239-151">DateTimeOffset</span></span>|<span data-ttu-id="90239-152">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="90239-152">Last update time</span></span>|
|<span data-ttu-id="90239-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="90239-153">configurationVersion</span></span>|<span data-ttu-id="90239-154">Int32</span><span class="sxs-lookup"><span data-stu-id="90239-154">Int32</span></span>|<span data-ttu-id="90239-155">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="90239-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="90239-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="90239-156">Response</span></span>
<span data-ttu-id="90239-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90239-157">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90239-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90239-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="90239-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90239-159">Request</span></span>
<span data-ttu-id="90239-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90239-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
Content-type: application/json
Content-length: 299

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="90239-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="90239-161">Response</span></span>
<span data-ttu-id="90239-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90239-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 348

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "9997c455-c455-9997-55c4-979955c49799",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```





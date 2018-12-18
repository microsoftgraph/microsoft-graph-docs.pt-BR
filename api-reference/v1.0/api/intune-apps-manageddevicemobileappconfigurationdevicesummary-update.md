---
title: Atualizar managedDeviceMobileAppConfigurationDeviceSummary
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationDeviceSummary.
author: tfitzmac
ms.openlocfilehash: 35a75cba4d67c23f5c011bfe7e75e23452d4c954
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330174"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="655de-103">Atualizar managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="655de-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="655de-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="655de-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="655de-105">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="655de-105">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="655de-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="655de-106">Prerequisites</span></span>
<span data-ttu-id="655de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="655de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="655de-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="655de-109">Permission type</span></span>|<span data-ttu-id="655de-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="655de-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="655de-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="655de-111">Delegated (work or school account)</span></span>|<span data-ttu-id="655de-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="655de-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="655de-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="655de-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="655de-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="655de-114">Not supported.</span></span>|
|<span data-ttu-id="655de-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="655de-115">Application</span></span>|<span data-ttu-id="655de-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="655de-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="655de-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="655de-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="655de-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="655de-118">Request headers</span></span>
|<span data-ttu-id="655de-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="655de-119">Header</span></span>|<span data-ttu-id="655de-120">Valor</span><span class="sxs-lookup"><span data-stu-id="655de-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="655de-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="655de-121">Authorization</span></span>|<span data-ttu-id="655de-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="655de-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="655de-123">Accept</span><span class="sxs-lookup"><span data-stu-id="655de-123">Accept</span></span>|<span data-ttu-id="655de-124">application/json</span><span class="sxs-lookup"><span data-stu-id="655de-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="655de-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="655de-125">Request body</span></span>
<span data-ttu-id="655de-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="655de-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="655de-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="655de-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="655de-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="655de-128">Property</span></span>|<span data-ttu-id="655de-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="655de-129">Type</span></span>|<span data-ttu-id="655de-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="655de-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="655de-131">id</span><span class="sxs-lookup"><span data-stu-id="655de-131">id</span></span>|<span data-ttu-id="655de-132">String</span><span class="sxs-lookup"><span data-stu-id="655de-132">String</span></span>|<span data-ttu-id="655de-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="655de-133">Key of the entity.</span></span>|
|<span data-ttu-id="655de-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="655de-134">pendingCount</span></span>|<span data-ttu-id="655de-135">Int32</span><span class="sxs-lookup"><span data-stu-id="655de-135">Int32</span></span>|<span data-ttu-id="655de-136">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="655de-136">Number of pending devices</span></span>|
|<span data-ttu-id="655de-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="655de-137">notApplicableCount</span></span>|<span data-ttu-id="655de-138">Int32</span><span class="sxs-lookup"><span data-stu-id="655de-138">Int32</span></span>|<span data-ttu-id="655de-139">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="655de-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="655de-140">successCount</span><span class="sxs-lookup"><span data-stu-id="655de-140">successCount</span></span>|<span data-ttu-id="655de-141">Int32</span><span class="sxs-lookup"><span data-stu-id="655de-141">Int32</span></span>|<span data-ttu-id="655de-142">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="655de-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="655de-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="655de-143">errorCount</span></span>|<span data-ttu-id="655de-144">Int32</span><span class="sxs-lookup"><span data-stu-id="655de-144">Int32</span></span>|<span data-ttu-id="655de-145">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="655de-145">Number of error devices</span></span>|
|<span data-ttu-id="655de-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="655de-146">failedCount</span></span>|<span data-ttu-id="655de-147">Int32</span><span class="sxs-lookup"><span data-stu-id="655de-147">Int32</span></span>|<span data-ttu-id="655de-148">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="655de-148">Number of failed devices</span></span>|
|<span data-ttu-id="655de-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="655de-149">lastUpdateDateTime</span></span>|<span data-ttu-id="655de-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="655de-150">DateTimeOffset</span></span>|<span data-ttu-id="655de-151">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="655de-151">Last update time</span></span>|
|<span data-ttu-id="655de-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="655de-152">configurationVersion</span></span>|<span data-ttu-id="655de-153">Int32</span><span class="sxs-lookup"><span data-stu-id="655de-153">Int32</span></span>|<span data-ttu-id="655de-154">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="655de-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="655de-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="655de-155">Response</span></span>
<span data-ttu-id="655de-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="655de-156">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="655de-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="655de-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="655de-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="655de-158">Request</span></span>
<span data-ttu-id="655de-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="655de-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="655de-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="655de-160">Response</span></span>
<span data-ttu-id="655de-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="655de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




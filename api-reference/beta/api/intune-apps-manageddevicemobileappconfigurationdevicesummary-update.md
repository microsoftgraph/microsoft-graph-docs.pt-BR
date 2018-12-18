---
title: Atualizar managedDeviceMobileAppConfigurationDeviceSummary
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationDeviceSummary.
author: tfitzmac
ms.openlocfilehash: a317582117e7bb270b7a197d99eb26dd1de1249e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360064"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="67baf-103">Atualizar managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="67baf-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="67baf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="67baf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67baf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="67baf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67baf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="67baf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67baf-107">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="67baf-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="67baf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67baf-108">Prerequisites</span></span>
<span data-ttu-id="67baf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67baf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67baf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67baf-111">Permission type</span></span>|<span data-ttu-id="67baf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67baf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67baf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67baf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67baf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67baf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="67baf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67baf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67baf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67baf-116">Not supported.</span></span>|
|<span data-ttu-id="67baf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67baf-117">Application</span></span>|<span data-ttu-id="67baf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67baf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67baf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67baf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="67baf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67baf-120">Request headers</span></span>
|<span data-ttu-id="67baf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67baf-121">Header</span></span>|<span data-ttu-id="67baf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="67baf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67baf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="67baf-123">Authorization</span></span>|<span data-ttu-id="67baf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67baf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67baf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="67baf-125">Accept</span></span>|<span data-ttu-id="67baf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67baf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67baf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67baf-127">Request body</span></span>
<span data-ttu-id="67baf-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="67baf-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="67baf-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="67baf-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="67baf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67baf-130">Property</span></span>|<span data-ttu-id="67baf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="67baf-131">Type</span></span>|<span data-ttu-id="67baf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="67baf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67baf-133">id</span><span class="sxs-lookup"><span data-stu-id="67baf-133">id</span></span>|<span data-ttu-id="67baf-134">String</span><span class="sxs-lookup"><span data-stu-id="67baf-134">String</span></span>|<span data-ttu-id="67baf-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="67baf-135">Key of the entity.</span></span>|
|<span data-ttu-id="67baf-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="67baf-136">pendingCount</span></span>|<span data-ttu-id="67baf-137">Int32</span><span class="sxs-lookup"><span data-stu-id="67baf-137">Int32</span></span>|<span data-ttu-id="67baf-138">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="67baf-138">Number of pending devices</span></span>|
|<span data-ttu-id="67baf-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="67baf-139">notApplicableCount</span></span>|<span data-ttu-id="67baf-140">Int32</span><span class="sxs-lookup"><span data-stu-id="67baf-140">Int32</span></span>|<span data-ttu-id="67baf-141">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="67baf-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="67baf-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="67baf-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="67baf-143">Int32</span><span class="sxs-lookup"><span data-stu-id="67baf-143">Int32</span></span>|<span data-ttu-id="67baf-144">Número de dispositivos não aplicáveis devido à plataforma de incompatibilidade e política</span><span class="sxs-lookup"><span data-stu-id="67baf-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="67baf-145">successCount</span><span class="sxs-lookup"><span data-stu-id="67baf-145">successCount</span></span>|<span data-ttu-id="67baf-146">Int32</span><span class="sxs-lookup"><span data-stu-id="67baf-146">Int32</span></span>|<span data-ttu-id="67baf-147">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="67baf-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="67baf-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="67baf-148">errorCount</span></span>|<span data-ttu-id="67baf-149">Int32</span><span class="sxs-lookup"><span data-stu-id="67baf-149">Int32</span></span>|<span data-ttu-id="67baf-150">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="67baf-150">Number of error devices</span></span>|
|<span data-ttu-id="67baf-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="67baf-151">failedCount</span></span>|<span data-ttu-id="67baf-152">Int32</span><span class="sxs-lookup"><span data-stu-id="67baf-152">Int32</span></span>|<span data-ttu-id="67baf-153">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="67baf-153">Number of failed devices</span></span>|
|<span data-ttu-id="67baf-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="67baf-154">conflictCount</span></span>|<span data-ttu-id="67baf-155">Int32</span><span class="sxs-lookup"><span data-stu-id="67baf-155">Int32</span></span>|<span data-ttu-id="67baf-156">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="67baf-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="67baf-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="67baf-157">lastUpdateDateTime</span></span>|<span data-ttu-id="67baf-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67baf-158">DateTimeOffset</span></span>|<span data-ttu-id="67baf-159">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="67baf-159">Last update time</span></span>|
|<span data-ttu-id="67baf-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="67baf-160">configurationVersion</span></span>|<span data-ttu-id="67baf-161">Int32</span><span class="sxs-lookup"><span data-stu-id="67baf-161">Int32</span></span>|<span data-ttu-id="67baf-162">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="67baf-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="67baf-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="67baf-163">Response</span></span>
<span data-ttu-id="67baf-164">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67baf-164">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67baf-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67baf-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="67baf-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67baf-166">Request</span></span>
<span data-ttu-id="67baf-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67baf-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
Content-type: application/json
Content-length: 273

{
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

### <a name="response"></a><span data-ttu-id="67baf-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="67baf-168">Response</span></span>
<span data-ttu-id="67baf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67baf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






---
title: Atualizar managedDeviceMobileAppConfigurationUserSummary
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationUserSummary.
ms.openlocfilehash: 179f2de37fab17a6ef37a60d00c6b2c566906f9c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003734"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="0be0e-103">Atualizar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="0be0e-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="0be0e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0be0e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0be0e-105">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="0be0e-105">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0be0e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0be0e-106">Prerequisites</span></span>
<span data-ttu-id="0be0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0be0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0be0e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0be0e-109">Permission type</span></span>|<span data-ttu-id="0be0e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0be0e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0be0e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0be0e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0be0e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be0e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0be0e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0be0e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0be0e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0be0e-114">Not supported.</span></span>|
|<span data-ttu-id="0be0e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0be0e-115">Application</span></span>|<span data-ttu-id="0be0e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0be0e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0be0e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0be0e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="0be0e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0be0e-118">Request headers</span></span>
|<span data-ttu-id="0be0e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0be0e-119">Header</span></span>|<span data-ttu-id="0be0e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0be0e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0be0e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0be0e-121">Authorization</span></span>|<span data-ttu-id="0be0e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0be0e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0be0e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0be0e-123">Accept</span></span>|<span data-ttu-id="0be0e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0be0e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0be0e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0be0e-125">Request body</span></span>
<span data-ttu-id="0be0e-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="0be0e-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="0be0e-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="0be0e-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="0be0e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0be0e-128">Property</span></span>|<span data-ttu-id="0be0e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0be0e-129">Type</span></span>|<span data-ttu-id="0be0e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0be0e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0be0e-131">id</span><span class="sxs-lookup"><span data-stu-id="0be0e-131">id</span></span>|<span data-ttu-id="0be0e-132">String</span><span class="sxs-lookup"><span data-stu-id="0be0e-132">String</span></span>|<span data-ttu-id="0be0e-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0be0e-133">Key of the entity.</span></span>|
|<span data-ttu-id="0be0e-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="0be0e-134">pendingCount</span></span>|<span data-ttu-id="0be0e-135">Int32</span><span class="sxs-lookup"><span data-stu-id="0be0e-135">Int32</span></span>|<span data-ttu-id="0be0e-136">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="0be0e-136">Number of pending Users</span></span>|
|<span data-ttu-id="0be0e-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="0be0e-137">notApplicableCount</span></span>|<span data-ttu-id="0be0e-138">Int32</span><span class="sxs-lookup"><span data-stu-id="0be0e-138">Int32</span></span>|<span data-ttu-id="0be0e-139">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="0be0e-139">Number of not applicable users</span></span>|
|<span data-ttu-id="0be0e-140">successCount</span><span class="sxs-lookup"><span data-stu-id="0be0e-140">successCount</span></span>|<span data-ttu-id="0be0e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="0be0e-141">Int32</span></span>|<span data-ttu-id="0be0e-142">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="0be0e-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="0be0e-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="0be0e-143">errorCount</span></span>|<span data-ttu-id="0be0e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="0be0e-144">Int32</span></span>|<span data-ttu-id="0be0e-145">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="0be0e-145">Number of error Users</span></span>|
|<span data-ttu-id="0be0e-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="0be0e-146">failedCount</span></span>|<span data-ttu-id="0be0e-147">Int32</span><span class="sxs-lookup"><span data-stu-id="0be0e-147">Int32</span></span>|<span data-ttu-id="0be0e-148">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="0be0e-148">Number of failed Users</span></span>|
|<span data-ttu-id="0be0e-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="0be0e-149">lastUpdateDateTime</span></span>|<span data-ttu-id="0be0e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0be0e-150">DateTimeOffset</span></span>|<span data-ttu-id="0be0e-151">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="0be0e-151">Last update time</span></span>|
|<span data-ttu-id="0be0e-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="0be0e-152">configurationVersion</span></span>|<span data-ttu-id="0be0e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0be0e-153">Int32</span></span>|<span data-ttu-id="0be0e-154">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="0be0e-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="0be0e-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="0be0e-155">Response</span></span>
<span data-ttu-id="0be0e-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0be0e-156">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0be0e-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0be0e-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="0be0e-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0be0e-158">Request</span></span>
<span data-ttu-id="0be0e-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0be0e-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
Content-type: application/json
Content-length: 297

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="0be0e-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="0be0e-160">Response</span></span>
<span data-ttu-id="0be0e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0be0e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "7b953742-3742-7b95-4237-957b4237957b",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




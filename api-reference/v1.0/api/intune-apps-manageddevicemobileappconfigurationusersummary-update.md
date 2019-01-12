---
title: Atualizar managedDeviceMobileAppConfigurationUserSummary
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationUserSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3033d0dcaa3859c96236e4c89e2c83f26f96f135
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986926"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="e0465-103">Atualizar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="e0465-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="e0465-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e0465-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0465-105">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="e0465-105">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0465-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e0465-106">Prerequisites</span></span>
<span data-ttu-id="e0465-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0465-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0465-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0465-109">Permission type</span></span>|<span data-ttu-id="e0465-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e0465-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0465-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0465-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e0465-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0465-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e0465-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0465-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0465-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0465-114">Not supported.</span></span>|
|<span data-ttu-id="e0465-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0465-115">Application</span></span>|<span data-ttu-id="e0465-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0465-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0465-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0465-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="e0465-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0465-118">Request headers</span></span>
|<span data-ttu-id="e0465-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e0465-119">Header</span></span>|<span data-ttu-id="e0465-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e0465-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0465-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0465-121">Authorization</span></span>|<span data-ttu-id="e0465-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0465-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0465-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e0465-123">Accept</span></span>|<span data-ttu-id="e0465-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e0465-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0465-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0465-125">Request body</span></span>
<span data-ttu-id="e0465-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="e0465-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="e0465-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="e0465-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="e0465-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0465-128">Property</span></span>|<span data-ttu-id="e0465-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0465-129">Type</span></span>|<span data-ttu-id="e0465-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0465-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0465-131">id</span><span class="sxs-lookup"><span data-stu-id="e0465-131">id</span></span>|<span data-ttu-id="e0465-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0465-132">String</span></span>|<span data-ttu-id="e0465-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e0465-133">Key of the entity.</span></span>|
|<span data-ttu-id="e0465-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="e0465-134">pendingCount</span></span>|<span data-ttu-id="e0465-135">Int32</span><span class="sxs-lookup"><span data-stu-id="e0465-135">Int32</span></span>|<span data-ttu-id="e0465-136">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="e0465-136">Number of pending Users</span></span>|
|<span data-ttu-id="e0465-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e0465-137">notApplicableCount</span></span>|<span data-ttu-id="e0465-138">Int32</span><span class="sxs-lookup"><span data-stu-id="e0465-138">Int32</span></span>|<span data-ttu-id="e0465-139">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="e0465-139">Number of not applicable users</span></span>|
|<span data-ttu-id="e0465-140">successCount</span><span class="sxs-lookup"><span data-stu-id="e0465-140">successCount</span></span>|<span data-ttu-id="e0465-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e0465-141">Int32</span></span>|<span data-ttu-id="e0465-142">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="e0465-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="e0465-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="e0465-143">errorCount</span></span>|<span data-ttu-id="e0465-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e0465-144">Int32</span></span>|<span data-ttu-id="e0465-145">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="e0465-145">Number of error Users</span></span>|
|<span data-ttu-id="e0465-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="e0465-146">failedCount</span></span>|<span data-ttu-id="e0465-147">Int32</span><span class="sxs-lookup"><span data-stu-id="e0465-147">Int32</span></span>|<span data-ttu-id="e0465-148">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="e0465-148">Number of failed Users</span></span>|
|<span data-ttu-id="e0465-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e0465-149">lastUpdateDateTime</span></span>|<span data-ttu-id="e0465-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0465-150">DateTimeOffset</span></span>|<span data-ttu-id="e0465-151">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="e0465-151">Last update time</span></span>|
|<span data-ttu-id="e0465-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="e0465-152">configurationVersion</span></span>|<span data-ttu-id="e0465-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e0465-153">Int32</span></span>|<span data-ttu-id="e0465-154">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="e0465-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="e0465-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0465-155">Response</span></span>
<span data-ttu-id="e0465-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0465-156">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0465-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0465-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0465-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0465-158">Request</span></span>
<span data-ttu-id="e0465-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0465-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e0465-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0465-160">Response</span></span>
<span data-ttu-id="e0465-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0465-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




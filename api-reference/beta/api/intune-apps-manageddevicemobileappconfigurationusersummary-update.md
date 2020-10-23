---
title: Atualizar managedDeviceMobileAppConfigurationUserSummary
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationUserSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 44a8377e2ac2a33ba0632fb29d5664927ea82d91
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699314"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="62a6c-103">Atualizar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="62a6c-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

<span data-ttu-id="62a6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62a6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62a6c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62a6c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62a6c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62a6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62a6c-107">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="62a6c-107">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62a6c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62a6c-108">Prerequisites</span></span>
<span data-ttu-id="62a6c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62a6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62a6c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62a6c-111">Permission type</span></span>|<span data-ttu-id="62a6c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62a6c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62a6c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62a6c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62a6c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62a6c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="62a6c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62a6c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62a6c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62a6c-116">Not supported.</span></span>|
|<span data-ttu-id="62a6c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62a6c-117">Application</span></span>|<span data-ttu-id="62a6c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62a6c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62a6c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62a6c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="62a6c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62a6c-120">Request headers</span></span>
|<span data-ttu-id="62a6c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62a6c-121">Header</span></span>|<span data-ttu-id="62a6c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="62a6c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62a6c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="62a6c-123">Authorization</span></span>|<span data-ttu-id="62a6c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62a6c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62a6c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62a6c-125">Accept</span></span>|<span data-ttu-id="62a6c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62a6c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62a6c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62a6c-127">Request body</span></span>
<span data-ttu-id="62a6c-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="62a6c-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="62a6c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="62a6c-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="62a6c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62a6c-130">Property</span></span>|<span data-ttu-id="62a6c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="62a6c-131">Type</span></span>|<span data-ttu-id="62a6c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="62a6c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62a6c-133">id</span><span class="sxs-lookup"><span data-stu-id="62a6c-133">id</span></span>|<span data-ttu-id="62a6c-134">String</span><span class="sxs-lookup"><span data-stu-id="62a6c-134">String</span></span>|<span data-ttu-id="62a6c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="62a6c-135">Key of the entity.</span></span>|
|<span data-ttu-id="62a6c-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="62a6c-136">pendingCount</span></span>|<span data-ttu-id="62a6c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="62a6c-137">Int32</span></span>|<span data-ttu-id="62a6c-138">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="62a6c-138">Number of pending Users</span></span>|
|<span data-ttu-id="62a6c-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="62a6c-139">notApplicableCount</span></span>|<span data-ttu-id="62a6c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="62a6c-140">Int32</span></span>|<span data-ttu-id="62a6c-141">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="62a6c-141">Number of not applicable users</span></span>|
|<span data-ttu-id="62a6c-142">successCount</span><span class="sxs-lookup"><span data-stu-id="62a6c-142">successCount</span></span>|<span data-ttu-id="62a6c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="62a6c-143">Int32</span></span>|<span data-ttu-id="62a6c-144">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="62a6c-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="62a6c-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="62a6c-145">errorCount</span></span>|<span data-ttu-id="62a6c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="62a6c-146">Int32</span></span>|<span data-ttu-id="62a6c-147">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="62a6c-147">Number of error Users</span></span>|
|<span data-ttu-id="62a6c-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="62a6c-148">failedCount</span></span>|<span data-ttu-id="62a6c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="62a6c-149">Int32</span></span>|<span data-ttu-id="62a6c-150">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="62a6c-150">Number of failed Users</span></span>|
|<span data-ttu-id="62a6c-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="62a6c-151">conflictCount</span></span>|<span data-ttu-id="62a6c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="62a6c-152">Int32</span></span>|<span data-ttu-id="62a6c-153">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="62a6c-153">Number of users in conflict</span></span>|
|<span data-ttu-id="62a6c-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="62a6c-154">lastUpdateDateTime</span></span>|<span data-ttu-id="62a6c-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62a6c-155">DateTimeOffset</span></span>|<span data-ttu-id="62a6c-156">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="62a6c-156">Last update time</span></span>|
|<span data-ttu-id="62a6c-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="62a6c-157">configurationVersion</span></span>|<span data-ttu-id="62a6c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="62a6c-158">Int32</span></span>|<span data-ttu-id="62a6c-159">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="62a6c-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="62a6c-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="62a6c-160">Response</span></span>
<span data-ttu-id="62a6c-161">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62a6c-161">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62a6c-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62a6c-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="62a6c-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62a6c-163">Request</span></span>
<span data-ttu-id="62a6c-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62a6c-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
Content-type: application/json
Content-length: 321

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="62a6c-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="62a6c-165">Response</span></span>
<span data-ttu-id="62a6c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62a6c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 370

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "7b953742-3742-7b95-4237-957b4237957b",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```






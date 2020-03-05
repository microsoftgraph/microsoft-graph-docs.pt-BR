---
title: Atualizar managedDeviceMobileAppConfigurationUserSummary
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationUserSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b7729480ca5322cbd8bb5d158c800ced30ee2f6f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450955"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="b7f06-103">Atualizar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="b7f06-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

<span data-ttu-id="b7f06-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b7f06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7f06-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b7f06-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7f06-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7f06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7f06-107">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="b7f06-107">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7f06-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7f06-108">Prerequisites</span></span>
<span data-ttu-id="b7f06-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7f06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7f06-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7f06-111">Permission type</span></span>|<span data-ttu-id="b7f06-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b7f06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7f06-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7f06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7f06-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7f06-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b7f06-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7f06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7f06-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7f06-116">Not supported.</span></span>|
|<span data-ttu-id="b7f06-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7f06-117">Application</span></span>|<span data-ttu-id="b7f06-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7f06-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7f06-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7f06-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="b7f06-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7f06-120">Request headers</span></span>
|<span data-ttu-id="b7f06-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7f06-121">Header</span></span>|<span data-ttu-id="b7f06-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b7f06-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7f06-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7f06-123">Authorization</span></span>|<span data-ttu-id="b7f06-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7f06-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7f06-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b7f06-125">Accept</span></span>|<span data-ttu-id="b7f06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7f06-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7f06-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7f06-127">Request body</span></span>
<span data-ttu-id="b7f06-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="b7f06-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="b7f06-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="b7f06-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="b7f06-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7f06-130">Property</span></span>|<span data-ttu-id="b7f06-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7f06-131">Type</span></span>|<span data-ttu-id="b7f06-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7f06-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7f06-133">id</span><span class="sxs-lookup"><span data-stu-id="b7f06-133">id</span></span>|<span data-ttu-id="b7f06-134">String</span><span class="sxs-lookup"><span data-stu-id="b7f06-134">String</span></span>|<span data-ttu-id="b7f06-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b7f06-135">Key of the entity.</span></span>|
|<span data-ttu-id="b7f06-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="b7f06-136">pendingCount</span></span>|<span data-ttu-id="b7f06-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f06-137">Int32</span></span>|<span data-ttu-id="b7f06-138">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="b7f06-138">Number of pending Users</span></span>|
|<span data-ttu-id="b7f06-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="b7f06-139">notApplicableCount</span></span>|<span data-ttu-id="b7f06-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f06-140">Int32</span></span>|<span data-ttu-id="b7f06-141">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="b7f06-141">Number of not applicable users</span></span>|
|<span data-ttu-id="b7f06-142">successCount</span><span class="sxs-lookup"><span data-stu-id="b7f06-142">successCount</span></span>|<span data-ttu-id="b7f06-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f06-143">Int32</span></span>|<span data-ttu-id="b7f06-144">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="b7f06-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="b7f06-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="b7f06-145">errorCount</span></span>|<span data-ttu-id="b7f06-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f06-146">Int32</span></span>|<span data-ttu-id="b7f06-147">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="b7f06-147">Number of error Users</span></span>|
|<span data-ttu-id="b7f06-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="b7f06-148">failedCount</span></span>|<span data-ttu-id="b7f06-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f06-149">Int32</span></span>|<span data-ttu-id="b7f06-150">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="b7f06-150">Number of failed Users</span></span>|
|<span data-ttu-id="b7f06-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="b7f06-151">conflictCount</span></span>|<span data-ttu-id="b7f06-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f06-152">Int32</span></span>|<span data-ttu-id="b7f06-153">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="b7f06-153">Number of users in conflict</span></span>|
|<span data-ttu-id="b7f06-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="b7f06-154">lastUpdateDateTime</span></span>|<span data-ttu-id="b7f06-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7f06-155">DateTimeOffset</span></span>|<span data-ttu-id="b7f06-156">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="b7f06-156">Last update time</span></span>|
|<span data-ttu-id="b7f06-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="b7f06-157">configurationVersion</span></span>|<span data-ttu-id="b7f06-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f06-158">Int32</span></span>|<span data-ttu-id="b7f06-159">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="b7f06-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="b7f06-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7f06-160">Response</span></span>
<span data-ttu-id="b7f06-161">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7f06-161">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7f06-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7f06-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7f06-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7f06-163">Request</span></span>
<span data-ttu-id="b7f06-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7f06-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b7f06-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7f06-165">Response</span></span>
<span data-ttu-id="b7f06-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7f06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






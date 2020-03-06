---
title: Atualizar deviceConfigurationDeviceOverview
description: Atualizar as propriedades de um objeto deviceConfigurationDeviceOverview.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 33f68bb41e2f22dac51f0805bb0b1305361446c4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514793"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="601a6-103">Atualizar deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="601a6-103">Update deviceConfigurationDeviceOverview</span></span>

<span data-ttu-id="601a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="601a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="601a6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="601a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="601a6-106">Atualizar as propriedades de um objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="601a6-106">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="601a6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="601a6-107">Prerequisites</span></span>
<span data-ttu-id="601a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="601a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="601a6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="601a6-110">Permission type</span></span>|<span data-ttu-id="601a6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="601a6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="601a6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="601a6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="601a6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="601a6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="601a6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="601a6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="601a6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="601a6-115">Not supported.</span></span>|
|<span data-ttu-id="601a6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="601a6-116">Application</span></span>|<span data-ttu-id="601a6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="601a6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="601a6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="601a6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="601a6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="601a6-119">Request headers</span></span>
|<span data-ttu-id="601a6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="601a6-120">Header</span></span>|<span data-ttu-id="601a6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="601a6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="601a6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="601a6-122">Authorization</span></span>|<span data-ttu-id="601a6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="601a6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="601a6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="601a6-124">Accept</span></span>|<span data-ttu-id="601a6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="601a6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="601a6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="601a6-126">Request body</span></span>
<span data-ttu-id="601a6-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="601a6-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="601a6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="601a6-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="601a6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="601a6-129">Property</span></span>|<span data-ttu-id="601a6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="601a6-130">Type</span></span>|<span data-ttu-id="601a6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="601a6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="601a6-132">id</span><span class="sxs-lookup"><span data-stu-id="601a6-132">id</span></span>|<span data-ttu-id="601a6-133">String</span><span class="sxs-lookup"><span data-stu-id="601a6-133">String</span></span>|<span data-ttu-id="601a6-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="601a6-134">Key of the entity.</span></span>|
|<span data-ttu-id="601a6-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="601a6-135">pendingCount</span></span>|<span data-ttu-id="601a6-136">Int32</span><span class="sxs-lookup"><span data-stu-id="601a6-136">Int32</span></span>|<span data-ttu-id="601a6-137">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="601a6-137">Number of pending devices</span></span>|
|<span data-ttu-id="601a6-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="601a6-138">notApplicableCount</span></span>|<span data-ttu-id="601a6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="601a6-139">Int32</span></span>|<span data-ttu-id="601a6-140">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="601a6-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="601a6-141">successCount</span><span class="sxs-lookup"><span data-stu-id="601a6-141">successCount</span></span>|<span data-ttu-id="601a6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="601a6-142">Int32</span></span>|<span data-ttu-id="601a6-143">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="601a6-143">Number of succeeded devices</span></span>|
|<span data-ttu-id="601a6-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="601a6-144">errorCount</span></span>|<span data-ttu-id="601a6-145">Int32</span><span class="sxs-lookup"><span data-stu-id="601a6-145">Int32</span></span>|<span data-ttu-id="601a6-146">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="601a6-146">Number of error devices</span></span>|
|<span data-ttu-id="601a6-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="601a6-147">failedCount</span></span>|<span data-ttu-id="601a6-148">Int32</span><span class="sxs-lookup"><span data-stu-id="601a6-148">Int32</span></span>|<span data-ttu-id="601a6-149">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="601a6-149">Number of failed devices</span></span>|
|<span data-ttu-id="601a6-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="601a6-150">lastUpdateDateTime</span></span>|<span data-ttu-id="601a6-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="601a6-151">DateTimeOffset</span></span>|<span data-ttu-id="601a6-152">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="601a6-152">Last update time</span></span>|
|<span data-ttu-id="601a6-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="601a6-153">configurationVersion</span></span>|<span data-ttu-id="601a6-154">Int32</span><span class="sxs-lookup"><span data-stu-id="601a6-154">Int32</span></span>|<span data-ttu-id="601a6-155">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="601a6-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="601a6-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="601a6-156">Response</span></span>
<span data-ttu-id="601a6-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="601a6-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="601a6-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="601a6-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="601a6-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="601a6-159">Request</span></span>
<span data-ttu-id="601a6-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="601a6-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 284

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="601a6-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="601a6-161">Response</span></span>
<span data-ttu-id="601a6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="601a6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 333

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```





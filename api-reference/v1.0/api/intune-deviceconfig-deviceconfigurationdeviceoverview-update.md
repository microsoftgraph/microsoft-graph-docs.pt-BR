---
title: Atualizar deviceConfigurationDeviceOverview
description: Atualizar as propriedades de um objeto deviceConfigurationDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0e47f904a5ee1216a63ed304411fca708995cc1e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017516"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="bcbcb-103">Atualizar deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="bcbcb-103">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="bcbcb-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bcbcb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcbcb-105">Atualizar as propriedades de um objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="bcbcb-105">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcbcb-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bcbcb-106">Prerequisites</span></span>
<span data-ttu-id="bcbcb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcbcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcbcb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bcbcb-109">Permission type</span></span>|<span data-ttu-id="bcbcb-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bcbcb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcbcb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bcbcb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bcbcb-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcbcb-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bcbcb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bcbcb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcbcb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcbcb-114">Not supported.</span></span>|
|<span data-ttu-id="bcbcb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bcbcb-115">Application</span></span>|<span data-ttu-id="bcbcb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcbcb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcbcb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcbcb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="bcbcb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bcbcb-118">Request headers</span></span>
|<span data-ttu-id="bcbcb-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bcbcb-119">Header</span></span>|<span data-ttu-id="bcbcb-120">Valor</span><span class="sxs-lookup"><span data-stu-id="bcbcb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcbcb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bcbcb-121">Authorization</span></span>|<span data-ttu-id="bcbcb-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bcbcb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcbcb-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bcbcb-123">Accept</span></span>|<span data-ttu-id="bcbcb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bcbcb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcbcb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcbcb-125">Request body</span></span>
<span data-ttu-id="bcbcb-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="bcbcb-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="bcbcb-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="bcbcb-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="bcbcb-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bcbcb-128">Property</span></span>|<span data-ttu-id="bcbcb-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcbcb-129">Type</span></span>|<span data-ttu-id="bcbcb-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcbcb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcbcb-131">id</span><span class="sxs-lookup"><span data-stu-id="bcbcb-131">id</span></span>|<span data-ttu-id="bcbcb-132">String</span><span class="sxs-lookup"><span data-stu-id="bcbcb-132">String</span></span>|<span data-ttu-id="bcbcb-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bcbcb-133">Key of the entity.</span></span>|
|<span data-ttu-id="bcbcb-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="bcbcb-134">pendingCount</span></span>|<span data-ttu-id="bcbcb-135">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbcb-135">Int32</span></span>|<span data-ttu-id="bcbcb-136">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="bcbcb-136">Number of pending devices</span></span>|
|<span data-ttu-id="bcbcb-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="bcbcb-137">notApplicableCount</span></span>|<span data-ttu-id="bcbcb-138">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbcb-138">Int32</span></span>|<span data-ttu-id="bcbcb-139">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="bcbcb-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="bcbcb-140">successCount</span><span class="sxs-lookup"><span data-stu-id="bcbcb-140">successCount</span></span>|<span data-ttu-id="bcbcb-141">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbcb-141">Int32</span></span>|<span data-ttu-id="bcbcb-142">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="bcbcb-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="bcbcb-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="bcbcb-143">errorCount</span></span>|<span data-ttu-id="bcbcb-144">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbcb-144">Int32</span></span>|<span data-ttu-id="bcbcb-145">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="bcbcb-145">Number of error devices</span></span>|
|<span data-ttu-id="bcbcb-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="bcbcb-146">failedCount</span></span>|<span data-ttu-id="bcbcb-147">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbcb-147">Int32</span></span>|<span data-ttu-id="bcbcb-148">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="bcbcb-148">Number of failed devices</span></span>|
|<span data-ttu-id="bcbcb-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="bcbcb-149">lastUpdateDateTime</span></span>|<span data-ttu-id="bcbcb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcbcb-150">DateTimeOffset</span></span>|<span data-ttu-id="bcbcb-151">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="bcbcb-151">Last update time</span></span>|
|<span data-ttu-id="bcbcb-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="bcbcb-152">configurationVersion</span></span>|<span data-ttu-id="bcbcb-153">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbcb-153">Int32</span></span>|<span data-ttu-id="bcbcb-154">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="bcbcb-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="bcbcb-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcbcb-155">Response</span></span>
<span data-ttu-id="bcbcb-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcbcb-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcbcb-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bcbcb-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcbcb-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcbcb-158">Request</span></span>
<span data-ttu-id="bcbcb-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcbcb-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bcbcb-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcbcb-160">Response</span></span>
<span data-ttu-id="bcbcb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bcbcb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




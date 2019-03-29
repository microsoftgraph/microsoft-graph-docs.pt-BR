---
title: Atualizar deviceConfigurationDeviceOverview
description: Atualizar as propriedades de um objeto deviceConfigurationDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a3a8c916581e24397bb2f86d164f2a49dea3fa7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968305"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="801ba-103">Atualizar deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="801ba-103">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="801ba-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="801ba-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="801ba-105">Atualizar as propriedades de um objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="801ba-105">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="801ba-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="801ba-106">Prerequisites</span></span>
<span data-ttu-id="801ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="801ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="801ba-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="801ba-109">Permission type</span></span>|<span data-ttu-id="801ba-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="801ba-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="801ba-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="801ba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="801ba-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="801ba-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="801ba-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="801ba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="801ba-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="801ba-114">Not supported.</span></span>|
|<span data-ttu-id="801ba-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="801ba-115">Application</span></span>|<span data-ttu-id="801ba-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="801ba-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="801ba-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="801ba-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="801ba-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="801ba-118">Request headers</span></span>
|<span data-ttu-id="801ba-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="801ba-119">Header</span></span>|<span data-ttu-id="801ba-120">Valor</span><span class="sxs-lookup"><span data-stu-id="801ba-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="801ba-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="801ba-121">Authorization</span></span>|<span data-ttu-id="801ba-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="801ba-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="801ba-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="801ba-123">Accept</span></span>|<span data-ttu-id="801ba-124">application/json</span><span class="sxs-lookup"><span data-stu-id="801ba-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="801ba-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="801ba-125">Request body</span></span>
<span data-ttu-id="801ba-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="801ba-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="801ba-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="801ba-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="801ba-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="801ba-128">Property</span></span>|<span data-ttu-id="801ba-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="801ba-129">Type</span></span>|<span data-ttu-id="801ba-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="801ba-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="801ba-131">id</span><span class="sxs-lookup"><span data-stu-id="801ba-131">id</span></span>|<span data-ttu-id="801ba-132">String</span><span class="sxs-lookup"><span data-stu-id="801ba-132">String</span></span>|<span data-ttu-id="801ba-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="801ba-133">Key of the entity.</span></span>|
|<span data-ttu-id="801ba-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="801ba-134">pendingCount</span></span>|<span data-ttu-id="801ba-135">Int32</span><span class="sxs-lookup"><span data-stu-id="801ba-135">Int32</span></span>|<span data-ttu-id="801ba-136">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="801ba-136">Number of pending devices</span></span>|
|<span data-ttu-id="801ba-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="801ba-137">notApplicableCount</span></span>|<span data-ttu-id="801ba-138">Int32</span><span class="sxs-lookup"><span data-stu-id="801ba-138">Int32</span></span>|<span data-ttu-id="801ba-139">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="801ba-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="801ba-140">successCount</span><span class="sxs-lookup"><span data-stu-id="801ba-140">successCount</span></span>|<span data-ttu-id="801ba-141">Int32</span><span class="sxs-lookup"><span data-stu-id="801ba-141">Int32</span></span>|<span data-ttu-id="801ba-142">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="801ba-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="801ba-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="801ba-143">errorCount</span></span>|<span data-ttu-id="801ba-144">Int32</span><span class="sxs-lookup"><span data-stu-id="801ba-144">Int32</span></span>|<span data-ttu-id="801ba-145">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="801ba-145">Number of error devices</span></span>|
|<span data-ttu-id="801ba-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="801ba-146">failedCount</span></span>|<span data-ttu-id="801ba-147">Int32</span><span class="sxs-lookup"><span data-stu-id="801ba-147">Int32</span></span>|<span data-ttu-id="801ba-148">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="801ba-148">Number of failed devices</span></span>|
|<span data-ttu-id="801ba-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="801ba-149">lastUpdateDateTime</span></span>|<span data-ttu-id="801ba-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="801ba-150">DateTimeOffset</span></span>|<span data-ttu-id="801ba-151">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="801ba-151">Last update time</span></span>|
|<span data-ttu-id="801ba-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="801ba-152">configurationVersion</span></span>|<span data-ttu-id="801ba-153">Int32</span><span class="sxs-lookup"><span data-stu-id="801ba-153">Int32</span></span>|<span data-ttu-id="801ba-154">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="801ba-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="801ba-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="801ba-155">Response</span></span>
<span data-ttu-id="801ba-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="801ba-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="801ba-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="801ba-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="801ba-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="801ba-158">Request</span></span>
<span data-ttu-id="801ba-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="801ba-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="801ba-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="801ba-160">Response</span></span>
<span data-ttu-id="801ba-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="801ba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




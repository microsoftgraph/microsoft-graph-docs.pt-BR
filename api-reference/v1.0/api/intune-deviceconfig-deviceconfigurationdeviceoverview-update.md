---
title: Atualizar deviceConfigurationDeviceOverview
description: Atualizar as propriedades de um objeto deviceConfigurationDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b199685d7fb173189701929adeec4ddd26bc21fe
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748345"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="bbe0a-103">Atualizar deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="bbe0a-103">Update deviceConfigurationDeviceOverview</span></span>

<span data-ttu-id="bbe0a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbe0a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbe0a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bbe0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbe0a-106">Atualizar as propriedades de um objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="bbe0a-106">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbe0a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bbe0a-107">Prerequisites</span></span>
<span data-ttu-id="bbe0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbe0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbe0a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbe0a-110">Permission type</span></span>|<span data-ttu-id="bbe0a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbe0a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbe0a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbe0a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bbe0a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbe0a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bbe0a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbe0a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbe0a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbe0a-115">Not supported.</span></span>|
|<span data-ttu-id="bbe0a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbe0a-116">Application</span></span>|<span data-ttu-id="bbe0a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbe0a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbe0a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbe0a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="bbe0a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbe0a-119">Request headers</span></span>
|<span data-ttu-id="bbe0a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bbe0a-120">Header</span></span>|<span data-ttu-id="bbe0a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bbe0a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbe0a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbe0a-122">Authorization</span></span>|<span data-ttu-id="bbe0a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbe0a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbe0a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bbe0a-124">Accept</span></span>|<span data-ttu-id="bbe0a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bbe0a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbe0a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbe0a-126">Request body</span></span>
<span data-ttu-id="bbe0a-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="bbe0a-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="bbe0a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="bbe0a-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="bbe0a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbe0a-129">Property</span></span>|<span data-ttu-id="bbe0a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbe0a-130">Type</span></span>|<span data-ttu-id="bbe0a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbe0a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbe0a-132">id</span><span class="sxs-lookup"><span data-stu-id="bbe0a-132">id</span></span>|<span data-ttu-id="bbe0a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbe0a-133">String</span></span>|<span data-ttu-id="bbe0a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bbe0a-134">Key of the entity.</span></span>|
|<span data-ttu-id="bbe0a-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="bbe0a-135">pendingCount</span></span>|<span data-ttu-id="bbe0a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="bbe0a-136">Int32</span></span>|<span data-ttu-id="bbe0a-137">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="bbe0a-137">Number of pending devices</span></span>|
|<span data-ttu-id="bbe0a-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="bbe0a-138">notApplicableCount</span></span>|<span data-ttu-id="bbe0a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="bbe0a-139">Int32</span></span>|<span data-ttu-id="bbe0a-140">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="bbe0a-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="bbe0a-141">successCount</span><span class="sxs-lookup"><span data-stu-id="bbe0a-141">successCount</span></span>|<span data-ttu-id="bbe0a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="bbe0a-142">Int32</span></span>|<span data-ttu-id="bbe0a-143">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="bbe0a-143">Number of succeeded devices</span></span>|
|<span data-ttu-id="bbe0a-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="bbe0a-144">errorCount</span></span>|<span data-ttu-id="bbe0a-145">Int32</span><span class="sxs-lookup"><span data-stu-id="bbe0a-145">Int32</span></span>|<span data-ttu-id="bbe0a-146">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="bbe0a-146">Number of error devices</span></span>|
|<span data-ttu-id="bbe0a-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="bbe0a-147">failedCount</span></span>|<span data-ttu-id="bbe0a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="bbe0a-148">Int32</span></span>|<span data-ttu-id="bbe0a-149">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="bbe0a-149">Number of failed devices</span></span>|
|<span data-ttu-id="bbe0a-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="bbe0a-150">lastUpdateDateTime</span></span>|<span data-ttu-id="bbe0a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbe0a-151">DateTimeOffset</span></span>|<span data-ttu-id="bbe0a-152">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="bbe0a-152">Last update time</span></span>|
|<span data-ttu-id="bbe0a-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="bbe0a-153">configurationVersion</span></span>|<span data-ttu-id="bbe0a-154">Int32</span><span class="sxs-lookup"><span data-stu-id="bbe0a-154">Int32</span></span>|<span data-ttu-id="bbe0a-155">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="bbe0a-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="bbe0a-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbe0a-156">Response</span></span>
<span data-ttu-id="bbe0a-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbe0a-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbe0a-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbe0a-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbe0a-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbe0a-159">Request</span></span>
<span data-ttu-id="bbe0a-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbe0a-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bbe0a-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbe0a-161">Response</span></span>
<span data-ttu-id="bbe0a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bbe0a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





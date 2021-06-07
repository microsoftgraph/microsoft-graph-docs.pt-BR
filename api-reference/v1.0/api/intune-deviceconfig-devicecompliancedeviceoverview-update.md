---
title: Atualizar deviceComplianceDeviceOverview
description: Atualizar as propriedades de um objeto deviceComplianceDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a24964891779a1b376bc4d0e92e013a1e1ca9728
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756642"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="3e518-103">Atualizar deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3e518-103">Update deviceComplianceDeviceOverview</span></span>

<span data-ttu-id="3e518-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e518-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e518-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3e518-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e518-106">Atualizar as propriedades de um objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="3e518-106">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e518-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3e518-107">Prerequisites</span></span>
<span data-ttu-id="3e518-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e518-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e518-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e518-110">Permission type</span></span>|<span data-ttu-id="3e518-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e518-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e518-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e518-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3e518-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e518-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e518-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e518-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e518-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e518-115">Not supported.</span></span>|
|<span data-ttu-id="3e518-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e518-116">Application</span></span>|<span data-ttu-id="3e518-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e518-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e518-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e518-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="3e518-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e518-119">Request headers</span></span>
|<span data-ttu-id="3e518-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3e518-120">Header</span></span>|<span data-ttu-id="3e518-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3e518-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e518-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e518-122">Authorization</span></span>|<span data-ttu-id="3e518-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e518-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e518-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3e518-124">Accept</span></span>|<span data-ttu-id="3e518-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3e518-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e518-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e518-126">Request body</span></span>
<span data-ttu-id="3e518-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="3e518-127">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="3e518-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="3e518-128">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="3e518-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e518-129">Property</span></span>|<span data-ttu-id="3e518-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e518-130">Type</span></span>|<span data-ttu-id="3e518-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e518-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e518-132">id</span><span class="sxs-lookup"><span data-stu-id="3e518-132">id</span></span>|<span data-ttu-id="3e518-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e518-133">String</span></span>|<span data-ttu-id="3e518-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3e518-134">Key of the entity.</span></span>|
|<span data-ttu-id="3e518-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="3e518-135">pendingCount</span></span>|<span data-ttu-id="3e518-136">Int32</span><span class="sxs-lookup"><span data-stu-id="3e518-136">Int32</span></span>|<span data-ttu-id="3e518-137">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="3e518-137">Number of pending devices</span></span>|
|<span data-ttu-id="3e518-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="3e518-138">notApplicableCount</span></span>|<span data-ttu-id="3e518-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3e518-139">Int32</span></span>|<span data-ttu-id="3e518-140">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="3e518-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="3e518-141">successCount</span><span class="sxs-lookup"><span data-stu-id="3e518-141">successCount</span></span>|<span data-ttu-id="3e518-142">Int32</span><span class="sxs-lookup"><span data-stu-id="3e518-142">Int32</span></span>|<span data-ttu-id="3e518-143">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="3e518-143">Number of succeeded devices</span></span>|
|<span data-ttu-id="3e518-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="3e518-144">errorCount</span></span>|<span data-ttu-id="3e518-145">Int32</span><span class="sxs-lookup"><span data-stu-id="3e518-145">Int32</span></span>|<span data-ttu-id="3e518-146">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="3e518-146">Number of error devices</span></span>|
|<span data-ttu-id="3e518-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="3e518-147">failedCount</span></span>|<span data-ttu-id="3e518-148">Int32</span><span class="sxs-lookup"><span data-stu-id="3e518-148">Int32</span></span>|<span data-ttu-id="3e518-149">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="3e518-149">Number of failed devices</span></span>|
|<span data-ttu-id="3e518-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="3e518-150">lastUpdateDateTime</span></span>|<span data-ttu-id="3e518-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e518-151">DateTimeOffset</span></span>|<span data-ttu-id="3e518-152">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="3e518-152">Last update time</span></span>|
|<span data-ttu-id="3e518-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="3e518-153">configurationVersion</span></span>|<span data-ttu-id="3e518-154">Int32</span><span class="sxs-lookup"><span data-stu-id="3e518-154">Int32</span></span>|<span data-ttu-id="3e518-155">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="3e518-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="3e518-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e518-156">Response</span></span>
<span data-ttu-id="3e518-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e518-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e518-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e518-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e518-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e518-159">Request</span></span>
<span data-ttu-id="3e518-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e518-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="3e518-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e518-161">Response</span></span>
<span data-ttu-id="3e518-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e518-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "886f167b-167b-886f-7b16-6f887b166f88",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```





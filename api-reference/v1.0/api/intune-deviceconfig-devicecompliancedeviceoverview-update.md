---
title: Atualizar deviceComplianceDeviceOverview
description: Atualizar as propriedades de um objeto deviceComplianceDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dafbfe048217320c0b82905b3c32d2cb9e179893
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572539"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="96519-103">Atualizar deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="96519-103">Update deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="96519-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96519-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96519-105">Atualizar as propriedades de um objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="96519-105">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96519-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96519-106">Prerequisites</span></span>
<span data-ttu-id="96519-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96519-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96519-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96519-109">Permission type</span></span>|<span data-ttu-id="96519-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="96519-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96519-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96519-111">Delegated (work or school account)</span></span>|<span data-ttu-id="96519-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96519-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="96519-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96519-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96519-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96519-114">Not supported.</span></span>|
|<span data-ttu-id="96519-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96519-115">Application</span></span>|<span data-ttu-id="96519-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96519-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96519-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96519-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="96519-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96519-118">Request headers</span></span>
|<span data-ttu-id="96519-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96519-119">Header</span></span>|<span data-ttu-id="96519-120">Valor</span><span class="sxs-lookup"><span data-stu-id="96519-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96519-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="96519-121">Authorization</span></span>|<span data-ttu-id="96519-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96519-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96519-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96519-123">Accept</span></span>|<span data-ttu-id="96519-124">application/json</span><span class="sxs-lookup"><span data-stu-id="96519-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96519-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96519-125">Request body</span></span>
<span data-ttu-id="96519-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="96519-126">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="96519-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="96519-127">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="96519-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96519-128">Property</span></span>|<span data-ttu-id="96519-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="96519-129">Type</span></span>|<span data-ttu-id="96519-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="96519-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96519-131">id</span><span class="sxs-lookup"><span data-stu-id="96519-131">id</span></span>|<span data-ttu-id="96519-132">String</span><span class="sxs-lookup"><span data-stu-id="96519-132">String</span></span>|<span data-ttu-id="96519-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="96519-133">Key of the entity.</span></span>|
|<span data-ttu-id="96519-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="96519-134">pendingCount</span></span>|<span data-ttu-id="96519-135">Int32</span><span class="sxs-lookup"><span data-stu-id="96519-135">Int32</span></span>|<span data-ttu-id="96519-136">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="96519-136">Number of pending devices</span></span>|
|<span data-ttu-id="96519-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="96519-137">notApplicableCount</span></span>|<span data-ttu-id="96519-138">Int32</span><span class="sxs-lookup"><span data-stu-id="96519-138">Int32</span></span>|<span data-ttu-id="96519-139">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="96519-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="96519-140">successCount</span><span class="sxs-lookup"><span data-stu-id="96519-140">successCount</span></span>|<span data-ttu-id="96519-141">Int32</span><span class="sxs-lookup"><span data-stu-id="96519-141">Int32</span></span>|<span data-ttu-id="96519-142">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="96519-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="96519-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="96519-143">errorCount</span></span>|<span data-ttu-id="96519-144">Int32</span><span class="sxs-lookup"><span data-stu-id="96519-144">Int32</span></span>|<span data-ttu-id="96519-145">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="96519-145">Number of error devices</span></span>|
|<span data-ttu-id="96519-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="96519-146">failedCount</span></span>|<span data-ttu-id="96519-147">Int32</span><span class="sxs-lookup"><span data-stu-id="96519-147">Int32</span></span>|<span data-ttu-id="96519-148">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="96519-148">Number of failed devices</span></span>|
|<span data-ttu-id="96519-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="96519-149">lastUpdateDateTime</span></span>|<span data-ttu-id="96519-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96519-150">DateTimeOffset</span></span>|<span data-ttu-id="96519-151">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="96519-151">Last update time</span></span>|
|<span data-ttu-id="96519-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="96519-152">configurationVersion</span></span>|<span data-ttu-id="96519-153">Int32</span><span class="sxs-lookup"><span data-stu-id="96519-153">Int32</span></span>|<span data-ttu-id="96519-154">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="96519-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="96519-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="96519-155">Response</span></span>
<span data-ttu-id="96519-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96519-156">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96519-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96519-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="96519-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96519-158">Request</span></span>
<span data-ttu-id="96519-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96519-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="96519-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="96519-160">Response</span></span>
<span data-ttu-id="96519-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96519-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




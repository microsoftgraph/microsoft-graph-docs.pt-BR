---
title: Atualizar settingStateDeviceSummary
description: Atualizar as propriedades de um objeto settingStateDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 61810538addfc22f371077214e9960bda2014e9e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458287"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="6191e-103">Atualizar settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6191e-103">Update settingStateDeviceSummary</span></span>

<span data-ttu-id="6191e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6191e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6191e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6191e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6191e-106">Atualizar as propriedades de um objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6191e-106">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6191e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6191e-107">Prerequisites</span></span>
<span data-ttu-id="6191e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6191e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6191e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6191e-110">Permission type</span></span>|<span data-ttu-id="6191e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6191e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6191e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6191e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6191e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6191e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6191e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6191e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6191e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6191e-115">Not supported.</span></span>|
|<span data-ttu-id="6191e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6191e-116">Application</span></span>|<span data-ttu-id="6191e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6191e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6191e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6191e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="6191e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6191e-119">Request headers</span></span>
|<span data-ttu-id="6191e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6191e-120">Header</span></span>|<span data-ttu-id="6191e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6191e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6191e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6191e-122">Authorization</span></span>|<span data-ttu-id="6191e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6191e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6191e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6191e-124">Accept</span></span>|<span data-ttu-id="6191e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6191e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6191e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6191e-126">Request body</span></span>
<span data-ttu-id="6191e-127">No corpo da solicitação, forneça uma representação JSON do objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6191e-127">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="6191e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6191e-128">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="6191e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6191e-129">Property</span></span>|<span data-ttu-id="6191e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6191e-130">Type</span></span>|<span data-ttu-id="6191e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6191e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6191e-132">id</span><span class="sxs-lookup"><span data-stu-id="6191e-132">id</span></span>|<span data-ttu-id="6191e-133">String</span><span class="sxs-lookup"><span data-stu-id="6191e-133">String</span></span>|<span data-ttu-id="6191e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6191e-134">Key of the entity.</span></span>|
|<span data-ttu-id="6191e-135">settingName</span><span class="sxs-lookup"><span data-stu-id="6191e-135">settingName</span></span>|<span data-ttu-id="6191e-136">String</span><span class="sxs-lookup"><span data-stu-id="6191e-136">String</span></span>|<span data-ttu-id="6191e-137">Nome da configuração</span><span class="sxs-lookup"><span data-stu-id="6191e-137">Name of the setting</span></span>|
|<span data-ttu-id="6191e-138">instancePath</span><span class="sxs-lookup"><span data-stu-id="6191e-138">instancePath</span></span>|<span data-ttu-id="6191e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6191e-139">String</span></span>|<span data-ttu-id="6191e-140">Nome de InstancePath para a configuração</span><span class="sxs-lookup"><span data-stu-id="6191e-140">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="6191e-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6191e-141">unknownDeviceCount</span></span>|<span data-ttu-id="6191e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6191e-142">Int32</span></span>|<span data-ttu-id="6191e-143">Contagem desconhecida de dispositivos para a configuração</span><span class="sxs-lookup"><span data-stu-id="6191e-143">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="6191e-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6191e-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="6191e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6191e-145">Int32</span></span>|<span data-ttu-id="6191e-146">Contagem não aplicável ao dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="6191e-146">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="6191e-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6191e-147">compliantDeviceCount</span></span>|<span data-ttu-id="6191e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="6191e-148">Int32</span></span>|<span data-ttu-id="6191e-149">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="6191e-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="6191e-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6191e-150">remediatedDeviceCount</span></span>|<span data-ttu-id="6191e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6191e-151">Int32</span></span>|<span data-ttu-id="6191e-152">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="6191e-152">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="6191e-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6191e-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="6191e-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6191e-154">Int32</span></span>|<span data-ttu-id="6191e-155">Contagem de dispositivo sem conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="6191e-155">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="6191e-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6191e-156">errorDeviceCount</span></span>|<span data-ttu-id="6191e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6191e-157">Int32</span></span>|<span data-ttu-id="6191e-158">Contagem de erros de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="6191e-158">Device error count for the setting</span></span>|
|<span data-ttu-id="6191e-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6191e-159">conflictDeviceCount</span></span>|<span data-ttu-id="6191e-160">Int32</span><span class="sxs-lookup"><span data-stu-id="6191e-160">Int32</span></span>|<span data-ttu-id="6191e-161">Contagem de erro de conflito de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="6191e-161">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="6191e-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="6191e-162">Response</span></span>
<span data-ttu-id="6191e-163">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6191e-163">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6191e-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6191e-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="6191e-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6191e-165">Request</span></span>
<span data-ttu-id="6191e-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6191e-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="6191e-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="6191e-167">Response</span></span>
<span data-ttu-id="6191e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6191e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```







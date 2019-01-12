---
title: Atualizar settingStateDeviceSummary
description: Atualizar as propriedades de um objeto settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 889466321037d72ab3f31d95deb3bd877ede7dbb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961439"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="994c5-103">Atualizar settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="994c5-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="994c5-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="994c5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="994c5-105">Atualizar as propriedades de um objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="994c5-105">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="994c5-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="994c5-106">Prerequisites</span></span>
<span data-ttu-id="994c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="994c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="994c5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="994c5-109">Permission type</span></span>|<span data-ttu-id="994c5-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="994c5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="994c5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="994c5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="994c5-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="994c5-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="994c5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="994c5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="994c5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="994c5-114">Not supported.</span></span>|
|<span data-ttu-id="994c5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="994c5-115">Application</span></span>|<span data-ttu-id="994c5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="994c5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="994c5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="994c5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="994c5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="994c5-118">Request headers</span></span>
|<span data-ttu-id="994c5-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="994c5-119">Header</span></span>|<span data-ttu-id="994c5-120">Valor</span><span class="sxs-lookup"><span data-stu-id="994c5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="994c5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="994c5-121">Authorization</span></span>|<span data-ttu-id="994c5-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="994c5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="994c5-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="994c5-123">Accept</span></span>|<span data-ttu-id="994c5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="994c5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="994c5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="994c5-125">Request body</span></span>
<span data-ttu-id="994c5-126">No corpo da solicitação, forneça uma representação JSON do objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="994c5-126">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="994c5-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="994c5-127">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="994c5-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="994c5-128">Property</span></span>|<span data-ttu-id="994c5-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="994c5-129">Type</span></span>|<span data-ttu-id="994c5-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="994c5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="994c5-131">id</span><span class="sxs-lookup"><span data-stu-id="994c5-131">id</span></span>|<span data-ttu-id="994c5-132">String</span><span class="sxs-lookup"><span data-stu-id="994c5-132">String</span></span>|<span data-ttu-id="994c5-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="994c5-133">Key of the entity.</span></span>|
|<span data-ttu-id="994c5-134">settingName</span><span class="sxs-lookup"><span data-stu-id="994c5-134">settingName</span></span>|<span data-ttu-id="994c5-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994c5-135">String</span></span>|<span data-ttu-id="994c5-136">Nome da configuração</span><span class="sxs-lookup"><span data-stu-id="994c5-136">Name of the setting</span></span>|
|<span data-ttu-id="994c5-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="994c5-137">instancePath</span></span>|<span data-ttu-id="994c5-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994c5-138">String</span></span>|<span data-ttu-id="994c5-139">Nome de InstancePath para a configuração</span><span class="sxs-lookup"><span data-stu-id="994c5-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="994c5-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="994c5-140">unknownDeviceCount</span></span>|<span data-ttu-id="994c5-141">Int32</span><span class="sxs-lookup"><span data-stu-id="994c5-141">Int32</span></span>|<span data-ttu-id="994c5-142">Contagem desconhecida de dispositivos para a configuração</span><span class="sxs-lookup"><span data-stu-id="994c5-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="994c5-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="994c5-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="994c5-144">Int32</span><span class="sxs-lookup"><span data-stu-id="994c5-144">Int32</span></span>|<span data-ttu-id="994c5-145">Contagem não aplicável ao dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="994c5-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="994c5-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="994c5-146">compliantDeviceCount</span></span>|<span data-ttu-id="994c5-147">Int32</span><span class="sxs-lookup"><span data-stu-id="994c5-147">Int32</span></span>|<span data-ttu-id="994c5-148">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="994c5-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="994c5-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="994c5-149">remediatedDeviceCount</span></span>|<span data-ttu-id="994c5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="994c5-150">Int32</span></span>|<span data-ttu-id="994c5-151">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="994c5-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="994c5-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="994c5-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="994c5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="994c5-153">Int32</span></span>|<span data-ttu-id="994c5-154">Contagem de dispositivo sem conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="994c5-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="994c5-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="994c5-155">errorDeviceCount</span></span>|<span data-ttu-id="994c5-156">Int32</span><span class="sxs-lookup"><span data-stu-id="994c5-156">Int32</span></span>|<span data-ttu-id="994c5-157">Contagem de erros de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="994c5-157">Device error count for the setting</span></span>|
|<span data-ttu-id="994c5-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="994c5-158">conflictDeviceCount</span></span>|<span data-ttu-id="994c5-159">Int32</span><span class="sxs-lookup"><span data-stu-id="994c5-159">Int32</span></span>|<span data-ttu-id="994c5-160">Contagem de erro de conflito de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="994c5-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="994c5-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="994c5-161">Response</span></span>
<span data-ttu-id="994c5-162">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="994c5-162">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="994c5-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="994c5-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="994c5-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="994c5-164">Request</span></span>
<span data-ttu-id="994c5-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="994c5-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="994c5-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="994c5-166">Response</span></span>
<span data-ttu-id="994c5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="994c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




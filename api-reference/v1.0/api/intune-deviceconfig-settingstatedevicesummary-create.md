---
title: Criar settingStateDeviceSummary
description: Criar um novo objeto settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2b91ab722e2918309d3b944b56f5c32ad6d463a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561149"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="0727e-103">Criar settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="0727e-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="0727e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0727e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0727e-105">Criar um novo objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="0727e-105">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0727e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0727e-106">Prerequisites</span></span>
<span data-ttu-id="0727e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0727e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0727e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0727e-109">Permission type</span></span>|<span data-ttu-id="0727e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0727e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0727e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0727e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0727e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0727e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0727e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0727e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0727e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0727e-114">Not supported.</span></span>|
|<span data-ttu-id="0727e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0727e-115">Application</span></span>|<span data-ttu-id="0727e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0727e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0727e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0727e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="0727e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0727e-118">Request headers</span></span>
|<span data-ttu-id="0727e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0727e-119">Header</span></span>|<span data-ttu-id="0727e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0727e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0727e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0727e-121">Authorization</span></span>|<span data-ttu-id="0727e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0727e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0727e-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0727e-123">Accept</span></span>|<span data-ttu-id="0727e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0727e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0727e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0727e-125">Request body</span></span>
<span data-ttu-id="0727e-126">No corpo da solicitação, forneça uma representação JSON do objeto settingStateDeviceSummary.</span><span class="sxs-lookup"><span data-stu-id="0727e-126">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="0727e-127">A tabela a seguir mostra as propriedades obrigatórias ao criar settingStateDeviceSummary.</span><span class="sxs-lookup"><span data-stu-id="0727e-127">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="0727e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0727e-128">Property</span></span>|<span data-ttu-id="0727e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0727e-129">Type</span></span>|<span data-ttu-id="0727e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0727e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0727e-131">id</span><span class="sxs-lookup"><span data-stu-id="0727e-131">id</span></span>|<span data-ttu-id="0727e-132">String</span><span class="sxs-lookup"><span data-stu-id="0727e-132">String</span></span>|<span data-ttu-id="0727e-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0727e-133">Key of the entity.</span></span>|
|<span data-ttu-id="0727e-134">settingName</span><span class="sxs-lookup"><span data-stu-id="0727e-134">settingName</span></span>|<span data-ttu-id="0727e-135">String</span><span class="sxs-lookup"><span data-stu-id="0727e-135">String</span></span>|<span data-ttu-id="0727e-136">Nome da configuração</span><span class="sxs-lookup"><span data-stu-id="0727e-136">Name of the setting</span></span>|
|<span data-ttu-id="0727e-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="0727e-137">instancePath</span></span>|<span data-ttu-id="0727e-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0727e-138">String</span></span>|<span data-ttu-id="0727e-139">Nome de InstancePath para a configuração</span><span class="sxs-lookup"><span data-stu-id="0727e-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="0727e-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0727e-140">unknownDeviceCount</span></span>|<span data-ttu-id="0727e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="0727e-141">Int32</span></span>|<span data-ttu-id="0727e-142">Contagem desconhecida de dispositivos para a configuração</span><span class="sxs-lookup"><span data-stu-id="0727e-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="0727e-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0727e-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="0727e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="0727e-144">Int32</span></span>|<span data-ttu-id="0727e-145">Contagem não aplicável ao dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="0727e-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="0727e-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0727e-146">compliantDeviceCount</span></span>|<span data-ttu-id="0727e-147">Int32</span><span class="sxs-lookup"><span data-stu-id="0727e-147">Int32</span></span>|<span data-ttu-id="0727e-148">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="0727e-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="0727e-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0727e-149">remediatedDeviceCount</span></span>|<span data-ttu-id="0727e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0727e-150">Int32</span></span>|<span data-ttu-id="0727e-151">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="0727e-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="0727e-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0727e-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="0727e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0727e-153">Int32</span></span>|<span data-ttu-id="0727e-154">Contagem de dispositivo sem conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="0727e-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="0727e-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0727e-155">errorDeviceCount</span></span>|<span data-ttu-id="0727e-156">Int32</span><span class="sxs-lookup"><span data-stu-id="0727e-156">Int32</span></span>|<span data-ttu-id="0727e-157">Contagem de erros de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="0727e-157">Device error count for the setting</span></span>|
|<span data-ttu-id="0727e-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0727e-158">conflictDeviceCount</span></span>|<span data-ttu-id="0727e-159">Int32</span><span class="sxs-lookup"><span data-stu-id="0727e-159">Int32</span></span>|<span data-ttu-id="0727e-160">Contagem de erro de conflito de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="0727e-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="0727e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="0727e-161">Response</span></span>
<span data-ttu-id="0727e-162">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0727e-162">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0727e-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0727e-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="0727e-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0727e-164">Request</span></span>
<span data-ttu-id="0727e-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0727e-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="0727e-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="0727e-166">Response</span></span>
<span data-ttu-id="0727e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0727e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




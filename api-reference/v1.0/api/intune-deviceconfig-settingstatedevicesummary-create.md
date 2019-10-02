---
title: Criar settingStateDeviceSummary
description: Criar um novo objeto settingStateDeviceSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a535f6a83be088b1798ee2baf3b8031cd69ddb9c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365842"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="babdb-103">Criar settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="babdb-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="babdb-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="babdb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="babdb-105">Criar um novo objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="babdb-105">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="babdb-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="babdb-106">Prerequisites</span></span>
<span data-ttu-id="babdb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="babdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="babdb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="babdb-109">Permission type</span></span>|<span data-ttu-id="babdb-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="babdb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="babdb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="babdb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="babdb-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="babdb-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="babdb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="babdb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="babdb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="babdb-114">Not supported.</span></span>|
|<span data-ttu-id="babdb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="babdb-115">Application</span></span>|<span data-ttu-id="babdb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="babdb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="babdb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="babdb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="babdb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="babdb-118">Request headers</span></span>
|<span data-ttu-id="babdb-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="babdb-119">Header</span></span>|<span data-ttu-id="babdb-120">Valor</span><span class="sxs-lookup"><span data-stu-id="babdb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="babdb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="babdb-121">Authorization</span></span>|<span data-ttu-id="babdb-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="babdb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="babdb-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="babdb-123">Accept</span></span>|<span data-ttu-id="babdb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="babdb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="babdb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="babdb-125">Request body</span></span>
<span data-ttu-id="babdb-126">No corpo da solicitação, forneça uma representação JSON do objeto settingStateDeviceSummary.</span><span class="sxs-lookup"><span data-stu-id="babdb-126">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="babdb-127">A tabela a seguir mostra as propriedades obrigatórias ao criar settingStateDeviceSummary.</span><span class="sxs-lookup"><span data-stu-id="babdb-127">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="babdb-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="babdb-128">Property</span></span>|<span data-ttu-id="babdb-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="babdb-129">Type</span></span>|<span data-ttu-id="babdb-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="babdb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="babdb-131">id</span><span class="sxs-lookup"><span data-stu-id="babdb-131">id</span></span>|<span data-ttu-id="babdb-132">String</span><span class="sxs-lookup"><span data-stu-id="babdb-132">String</span></span>|<span data-ttu-id="babdb-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="babdb-133">Key of the entity.</span></span>|
|<span data-ttu-id="babdb-134">settingName</span><span class="sxs-lookup"><span data-stu-id="babdb-134">settingName</span></span>|<span data-ttu-id="babdb-135">String</span><span class="sxs-lookup"><span data-stu-id="babdb-135">String</span></span>|<span data-ttu-id="babdb-136">Nome da configuração</span><span class="sxs-lookup"><span data-stu-id="babdb-136">Name of the setting</span></span>|
|<span data-ttu-id="babdb-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="babdb-137">instancePath</span></span>|<span data-ttu-id="babdb-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="babdb-138">String</span></span>|<span data-ttu-id="babdb-139">Nome de InstancePath para a configuração</span><span class="sxs-lookup"><span data-stu-id="babdb-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="babdb-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="babdb-140">unknownDeviceCount</span></span>|<span data-ttu-id="babdb-141">Int32</span><span class="sxs-lookup"><span data-stu-id="babdb-141">Int32</span></span>|<span data-ttu-id="babdb-142">Contagem desconhecida de dispositivos para a configuração</span><span class="sxs-lookup"><span data-stu-id="babdb-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="babdb-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="babdb-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="babdb-144">Int32</span><span class="sxs-lookup"><span data-stu-id="babdb-144">Int32</span></span>|<span data-ttu-id="babdb-145">Contagem não aplicável ao dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="babdb-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="babdb-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="babdb-146">compliantDeviceCount</span></span>|<span data-ttu-id="babdb-147">Int32</span><span class="sxs-lookup"><span data-stu-id="babdb-147">Int32</span></span>|<span data-ttu-id="babdb-148">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="babdb-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="babdb-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="babdb-149">remediatedDeviceCount</span></span>|<span data-ttu-id="babdb-150">Int32</span><span class="sxs-lookup"><span data-stu-id="babdb-150">Int32</span></span>|<span data-ttu-id="babdb-151">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="babdb-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="babdb-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="babdb-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="babdb-153">Int32</span><span class="sxs-lookup"><span data-stu-id="babdb-153">Int32</span></span>|<span data-ttu-id="babdb-154">Contagem de dispositivo sem conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="babdb-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="babdb-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="babdb-155">errorDeviceCount</span></span>|<span data-ttu-id="babdb-156">Int32</span><span class="sxs-lookup"><span data-stu-id="babdb-156">Int32</span></span>|<span data-ttu-id="babdb-157">Contagem de erros de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="babdb-157">Device error count for the setting</span></span>|
|<span data-ttu-id="babdb-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="babdb-158">conflictDeviceCount</span></span>|<span data-ttu-id="babdb-159">Int32</span><span class="sxs-lookup"><span data-stu-id="babdb-159">Int32</span></span>|<span data-ttu-id="babdb-160">Contagem de erro de conflito de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="babdb-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="babdb-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="babdb-161">Response</span></span>
<span data-ttu-id="babdb-162">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="babdb-162">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="babdb-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="babdb-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="babdb-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="babdb-164">Request</span></span>
<span data-ttu-id="babdb-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="babdb-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="babdb-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="babdb-166">Response</span></span>
<span data-ttu-id="babdb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="babdb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





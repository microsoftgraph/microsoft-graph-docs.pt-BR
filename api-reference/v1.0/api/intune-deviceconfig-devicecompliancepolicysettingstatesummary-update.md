---
title: Atualizar deviceCompliancePolicySettingStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicySettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 407fd8e16a1bdb9b94864b46897f18284c780c2a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756614"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="a3f66-103">Atualizar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="a3f66-103">Update deviceCompliancePolicySettingStateSummary</span></span>

<span data-ttu-id="a3f66-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3f66-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3f66-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a3f66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3f66-106">Atualizar as propriedades de um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a3f66-106">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3f66-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a3f66-107">Prerequisites</span></span>
<span data-ttu-id="a3f66-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3f66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3f66-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3f66-110">Permission type</span></span>|<span data-ttu-id="a3f66-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3f66-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3f66-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3f66-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3f66-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3f66-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3f66-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3f66-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3f66-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3f66-115">Not supported.</span></span>|
|<span data-ttu-id="a3f66-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3f66-116">Application</span></span>|<span data-ttu-id="a3f66-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3f66-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3f66-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3f66-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="a3f66-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3f66-119">Request headers</span></span>
|<span data-ttu-id="a3f66-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3f66-120">Header</span></span>|<span data-ttu-id="a3f66-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a3f66-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3f66-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3f66-122">Authorization</span></span>|<span data-ttu-id="a3f66-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3f66-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3f66-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a3f66-124">Accept</span></span>|<span data-ttu-id="a3f66-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3f66-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3f66-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3f66-126">Request body</span></span>
<span data-ttu-id="a3f66-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a3f66-127">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="a3f66-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a3f66-128">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="a3f66-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3f66-129">Property</span></span>|<span data-ttu-id="a3f66-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3f66-130">Type</span></span>|<span data-ttu-id="a3f66-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3f66-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3f66-132">id</span><span class="sxs-lookup"><span data-stu-id="a3f66-132">id</span></span>|<span data-ttu-id="a3f66-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3f66-133">String</span></span>|<span data-ttu-id="a3f66-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a3f66-134">Key of the entity.</span></span>|
|<span data-ttu-id="a3f66-135">configuração</span><span class="sxs-lookup"><span data-stu-id="a3f66-135">setting</span></span>|<span data-ttu-id="a3f66-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3f66-136">String</span></span>|<span data-ttu-id="a3f66-137">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="a3f66-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="a3f66-138">settingName</span><span class="sxs-lookup"><span data-stu-id="a3f66-138">settingName</span></span>|<span data-ttu-id="a3f66-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3f66-139">String</span></span>|<span data-ttu-id="a3f66-140">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="a3f66-140">Name of the setting.</span></span>|
|<span data-ttu-id="a3f66-141">platformType</span><span class="sxs-lookup"><span data-stu-id="a3f66-141">platformType</span></span>|[<span data-ttu-id="a3f66-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="a3f66-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="a3f66-143">Plataforma de configuração.</span><span class="sxs-lookup"><span data-stu-id="a3f66-143">Setting platform.</span></span> <span data-ttu-id="a3f66-144">Os valores possíveis são: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="a3f66-144">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="a3f66-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3f66-145">unknownDeviceCount</span></span>|<span data-ttu-id="a3f66-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a3f66-146">Int32</span></span>|<span data-ttu-id="a3f66-147">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="a3f66-147">Number of unknown devices</span></span>|
|<span data-ttu-id="a3f66-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3f66-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="a3f66-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a3f66-149">Int32</span></span>|<span data-ttu-id="a3f66-150">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="a3f66-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="a3f66-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3f66-151">compliantDeviceCount</span></span>|<span data-ttu-id="a3f66-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a3f66-152">Int32</span></span>|<span data-ttu-id="a3f66-153">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="a3f66-153">Number of compliant devices</span></span>|
|<span data-ttu-id="a3f66-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3f66-154">remediatedDeviceCount</span></span>|<span data-ttu-id="a3f66-155">Int32</span><span class="sxs-lookup"><span data-stu-id="a3f66-155">Int32</span></span>|<span data-ttu-id="a3f66-156">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="a3f66-156">Number of remediated devices</span></span>|
|<span data-ttu-id="a3f66-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3f66-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a3f66-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a3f66-158">Int32</span></span>|<span data-ttu-id="a3f66-159">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="a3f66-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="a3f66-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3f66-160">errorDeviceCount</span></span>|<span data-ttu-id="a3f66-161">Int32</span><span class="sxs-lookup"><span data-stu-id="a3f66-161">Int32</span></span>|<span data-ttu-id="a3f66-162">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="a3f66-162">Number of error devices</span></span>|
|<span data-ttu-id="a3f66-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3f66-163">conflictDeviceCount</span></span>|<span data-ttu-id="a3f66-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a3f66-164">Int32</span></span>|<span data-ttu-id="a3f66-165">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="a3f66-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="a3f66-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3f66-166">Response</span></span>
<span data-ttu-id="a3f66-167">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3f66-167">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3f66-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3f66-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3f66-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3f66-169">Request</span></span>
<span data-ttu-id="a3f66-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3f66-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="a3f66-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3f66-171">Response</span></span>
<span data-ttu-id="a3f66-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3f66-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```





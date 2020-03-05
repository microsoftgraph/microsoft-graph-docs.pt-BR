---
title: Atualizar deviceCompliancePolicySettingStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicySettingStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10f269b7db39d15eb008fa5a26dd513f8fdc2de5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443178"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="0b819-103">Atualizar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="0b819-103">Update deviceCompliancePolicySettingStateSummary</span></span>

<span data-ttu-id="0b819-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0b819-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b819-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0b819-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b819-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b819-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b819-107">Atualizar as propriedades de um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="0b819-107">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b819-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b819-108">Prerequisites</span></span>
<span data-ttu-id="0b819-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b819-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b819-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b819-111">Permission type</span></span>|<span data-ttu-id="0b819-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b819-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b819-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b819-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b819-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b819-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b819-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b819-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b819-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b819-116">Not supported.</span></span>|
|<span data-ttu-id="0b819-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b819-117">Application</span></span>|<span data-ttu-id="0b819-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b819-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b819-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b819-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="0b819-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b819-120">Request headers</span></span>
|<span data-ttu-id="0b819-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b819-121">Header</span></span>|<span data-ttu-id="0b819-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0b819-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b819-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b819-123">Authorization</span></span>|<span data-ttu-id="0b819-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b819-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b819-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0b819-125">Accept</span></span>|<span data-ttu-id="0b819-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b819-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b819-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b819-127">Request body</span></span>
<span data-ttu-id="0b819-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="0b819-128">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="0b819-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="0b819-129">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="0b819-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b819-130">Property</span></span>|<span data-ttu-id="0b819-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b819-131">Type</span></span>|<span data-ttu-id="0b819-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b819-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b819-133">id</span><span class="sxs-lookup"><span data-stu-id="0b819-133">id</span></span>|<span data-ttu-id="0b819-134">String</span><span class="sxs-lookup"><span data-stu-id="0b819-134">String</span></span>|<span data-ttu-id="0b819-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0b819-135">Key of the entity.</span></span>|
|<span data-ttu-id="0b819-136">configuração</span><span class="sxs-lookup"><span data-stu-id="0b819-136">setting</span></span>|<span data-ttu-id="0b819-137">String</span><span class="sxs-lookup"><span data-stu-id="0b819-137">String</span></span>|<span data-ttu-id="0b819-138">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="0b819-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="0b819-139">settingName</span><span class="sxs-lookup"><span data-stu-id="0b819-139">settingName</span></span>|<span data-ttu-id="0b819-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b819-140">String</span></span>|<span data-ttu-id="0b819-141">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="0b819-141">Name of the setting.</span></span>|
|<span data-ttu-id="0b819-142">platformType</span><span class="sxs-lookup"><span data-stu-id="0b819-142">platformType</span></span>|[<span data-ttu-id="0b819-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="0b819-143">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="0b819-144">Configuração de plataforma.</span><span class="sxs-lookup"><span data-stu-id="0b819-144">Setting platform.</span></span> <span data-ttu-id="0b819-145">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="0b819-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="0b819-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b819-146">unknownDeviceCount</span></span>|<span data-ttu-id="0b819-147">Int32</span><span class="sxs-lookup"><span data-stu-id="0b819-147">Int32</span></span>|<span data-ttu-id="0b819-148">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="0b819-148">Number of unknown devices</span></span>|
|<span data-ttu-id="0b819-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b819-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="0b819-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0b819-150">Int32</span></span>|<span data-ttu-id="0b819-151">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="0b819-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="0b819-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b819-152">compliantDeviceCount</span></span>|<span data-ttu-id="0b819-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0b819-153">Int32</span></span>|<span data-ttu-id="0b819-154">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="0b819-154">Number of compliant devices</span></span>|
|<span data-ttu-id="0b819-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b819-155">remediatedDeviceCount</span></span>|<span data-ttu-id="0b819-156">Int32</span><span class="sxs-lookup"><span data-stu-id="0b819-156">Int32</span></span>|<span data-ttu-id="0b819-157">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="0b819-157">Number of remediated devices</span></span>|
|<span data-ttu-id="0b819-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b819-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="0b819-159">Int32</span><span class="sxs-lookup"><span data-stu-id="0b819-159">Int32</span></span>|<span data-ttu-id="0b819-160">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="0b819-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="0b819-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b819-161">errorDeviceCount</span></span>|<span data-ttu-id="0b819-162">Int32</span><span class="sxs-lookup"><span data-stu-id="0b819-162">Int32</span></span>|<span data-ttu-id="0b819-163">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="0b819-163">Number of error devices</span></span>|
|<span data-ttu-id="0b819-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b819-164">conflictDeviceCount</span></span>|<span data-ttu-id="0b819-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0b819-165">Int32</span></span>|<span data-ttu-id="0b819-166">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="0b819-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="0b819-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b819-167">Response</span></span>
<span data-ttu-id="0b819-168">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b819-168">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b819-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b819-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b819-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b819-170">Request</span></span>
<span data-ttu-id="0b819-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b819-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "androidForWork",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="0b819-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b819-172">Response</span></span>
<span data-ttu-id="0b819-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b819-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "androidForWork",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```






---
title: Atualizar deviceCompliancePolicySettingStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 97eec7bba67552c21c208ed087aab40a096d47b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830020"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="565ea-103">Atualizar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="565ea-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="565ea-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="565ea-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="565ea-105">Atualizar as propriedades de um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="565ea-105">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="565ea-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="565ea-106">Prerequisites</span></span>
<span data-ttu-id="565ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="565ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="565ea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="565ea-109">Permission type</span></span>|<span data-ttu-id="565ea-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="565ea-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="565ea-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="565ea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="565ea-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="565ea-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="565ea-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="565ea-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="565ea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="565ea-114">Not supported.</span></span>|
|<span data-ttu-id="565ea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="565ea-115">Application</span></span>|<span data-ttu-id="565ea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="565ea-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="565ea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="565ea-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="565ea-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="565ea-118">Request headers</span></span>
|<span data-ttu-id="565ea-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="565ea-119">Header</span></span>|<span data-ttu-id="565ea-120">Valor</span><span class="sxs-lookup"><span data-stu-id="565ea-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="565ea-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="565ea-121">Authorization</span></span>|<span data-ttu-id="565ea-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="565ea-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="565ea-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="565ea-123">Accept</span></span>|<span data-ttu-id="565ea-124">application/json</span><span class="sxs-lookup"><span data-stu-id="565ea-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="565ea-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="565ea-125">Request body</span></span>
<span data-ttu-id="565ea-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="565ea-126">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="565ea-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="565ea-127">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="565ea-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="565ea-128">Property</span></span>|<span data-ttu-id="565ea-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="565ea-129">Type</span></span>|<span data-ttu-id="565ea-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="565ea-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="565ea-131">id</span><span class="sxs-lookup"><span data-stu-id="565ea-131">id</span></span>|<span data-ttu-id="565ea-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ea-132">String</span></span>|<span data-ttu-id="565ea-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="565ea-133">Key of the entity.</span></span>|
|<span data-ttu-id="565ea-134">configuração</span><span class="sxs-lookup"><span data-stu-id="565ea-134">setting</span></span>|<span data-ttu-id="565ea-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ea-135">String</span></span>|<span data-ttu-id="565ea-136">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="565ea-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="565ea-137">settingName</span><span class="sxs-lookup"><span data-stu-id="565ea-137">settingName</span></span>|<span data-ttu-id="565ea-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ea-138">String</span></span>|<span data-ttu-id="565ea-139">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="565ea-139">Name of the setting.</span></span>|
|<span data-ttu-id="565ea-140">platformType</span><span class="sxs-lookup"><span data-stu-id="565ea-140">platformType</span></span>|[<span data-ttu-id="565ea-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="565ea-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="565ea-142">Plataforma de configuração.</span><span class="sxs-lookup"><span data-stu-id="565ea-142">Setting platform.</span></span> <span data-ttu-id="565ea-143">Os valores possíveis são: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="565ea-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="565ea-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="565ea-144">unknownDeviceCount</span></span>|<span data-ttu-id="565ea-145">Int32</span><span class="sxs-lookup"><span data-stu-id="565ea-145">Int32</span></span>|<span data-ttu-id="565ea-146">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="565ea-146">Number of unknown devices</span></span>|
|<span data-ttu-id="565ea-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="565ea-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="565ea-148">Int32</span><span class="sxs-lookup"><span data-stu-id="565ea-148">Int32</span></span>|<span data-ttu-id="565ea-149">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="565ea-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="565ea-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="565ea-150">compliantDeviceCount</span></span>|<span data-ttu-id="565ea-151">Int32</span><span class="sxs-lookup"><span data-stu-id="565ea-151">Int32</span></span>|<span data-ttu-id="565ea-152">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="565ea-152">Number of compliant devices</span></span>|
|<span data-ttu-id="565ea-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="565ea-153">remediatedDeviceCount</span></span>|<span data-ttu-id="565ea-154">Int32</span><span class="sxs-lookup"><span data-stu-id="565ea-154">Int32</span></span>|<span data-ttu-id="565ea-155">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="565ea-155">Number of remediated devices</span></span>|
|<span data-ttu-id="565ea-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="565ea-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="565ea-157">Int32</span><span class="sxs-lookup"><span data-stu-id="565ea-157">Int32</span></span>|<span data-ttu-id="565ea-158">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="565ea-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="565ea-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="565ea-159">errorDeviceCount</span></span>|<span data-ttu-id="565ea-160">Int32</span><span class="sxs-lookup"><span data-stu-id="565ea-160">Int32</span></span>|<span data-ttu-id="565ea-161">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="565ea-161">Number of error devices</span></span>|
|<span data-ttu-id="565ea-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="565ea-162">conflictDeviceCount</span></span>|<span data-ttu-id="565ea-163">Int32</span><span class="sxs-lookup"><span data-stu-id="565ea-163">Int32</span></span>|<span data-ttu-id="565ea-164">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="565ea-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="565ea-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="565ea-165">Response</span></span>
<span data-ttu-id="565ea-166">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="565ea-166">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="565ea-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="565ea-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="565ea-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="565ea-168">Request</span></span>
<span data-ttu-id="565ea-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="565ea-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="565ea-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="565ea-170">Response</span></span>
<span data-ttu-id="565ea-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="565ea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




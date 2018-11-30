---
title: Criar deviceCompliancePolicySettingStateSummary
description: Crie um novo objeto deviceCompliancePolicySettingStateSummary.
ms.openlocfilehash: f7924b8ec3e8c32ccd62899a8576d56c85f0b233
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006803"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="b3795-103">Criar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="b3795-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="b3795-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b3795-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3795-105">Crie um novo objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="b3795-105">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3795-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b3795-106">Prerequisites</span></span>
<span data-ttu-id="b3795-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3795-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3795-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3795-109">Permission type</span></span>|<span data-ttu-id="b3795-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b3795-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3795-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3795-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b3795-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3795-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3795-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3795-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3795-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3795-114">Not supported.</span></span>|
|<span data-ttu-id="b3795-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3795-115">Application</span></span>|<span data-ttu-id="b3795-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3795-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3795-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3795-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="b3795-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3795-118">Request headers</span></span>
|<span data-ttu-id="b3795-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3795-119">Header</span></span>|<span data-ttu-id="b3795-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b3795-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3795-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3795-121">Authorization</span></span>|<span data-ttu-id="b3795-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3795-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3795-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b3795-123">Accept</span></span>|<span data-ttu-id="b3795-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b3795-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3795-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3795-125">Request body</span></span>
<span data-ttu-id="b3795-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="b3795-126">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="b3795-127">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="b3795-127">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="b3795-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3795-128">Property</span></span>|<span data-ttu-id="b3795-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3795-129">Type</span></span>|<span data-ttu-id="b3795-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3795-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3795-131">id</span><span class="sxs-lookup"><span data-stu-id="b3795-131">id</span></span>|<span data-ttu-id="b3795-132">String</span><span class="sxs-lookup"><span data-stu-id="b3795-132">String</span></span>|<span data-ttu-id="b3795-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b3795-133">Key of the entity.</span></span>|
|<span data-ttu-id="b3795-134">configuração</span><span class="sxs-lookup"><span data-stu-id="b3795-134">setting</span></span>|<span data-ttu-id="b3795-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3795-135">String</span></span>|<span data-ttu-id="b3795-136">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="b3795-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="b3795-137">settingName</span><span class="sxs-lookup"><span data-stu-id="b3795-137">settingName</span></span>|<span data-ttu-id="b3795-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3795-138">String</span></span>|<span data-ttu-id="b3795-139">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="b3795-139">Name of the setting.</span></span>|
|<span data-ttu-id="b3795-140">platformType</span><span class="sxs-lookup"><span data-stu-id="b3795-140">platformType</span></span>|[<span data-ttu-id="b3795-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="b3795-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="b3795-142">Plataforma de configuração.</span><span class="sxs-lookup"><span data-stu-id="b3795-142">Setting platform.</span></span> <span data-ttu-id="b3795-143">Os valores possíveis são: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="b3795-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="b3795-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b3795-144">unknownDeviceCount</span></span>|<span data-ttu-id="b3795-145">Int32</span><span class="sxs-lookup"><span data-stu-id="b3795-145">Int32</span></span>|<span data-ttu-id="b3795-146">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="b3795-146">Number of unknown devices</span></span>|
|<span data-ttu-id="b3795-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b3795-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="b3795-148">Int32</span><span class="sxs-lookup"><span data-stu-id="b3795-148">Int32</span></span>|<span data-ttu-id="b3795-149">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="b3795-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="b3795-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b3795-150">compliantDeviceCount</span></span>|<span data-ttu-id="b3795-151">Int32</span><span class="sxs-lookup"><span data-stu-id="b3795-151">Int32</span></span>|<span data-ttu-id="b3795-152">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="b3795-152">Number of compliant devices</span></span>|
|<span data-ttu-id="b3795-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b3795-153">remediatedDeviceCount</span></span>|<span data-ttu-id="b3795-154">Int32</span><span class="sxs-lookup"><span data-stu-id="b3795-154">Int32</span></span>|<span data-ttu-id="b3795-155">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="b3795-155">Number of remediated devices</span></span>|
|<span data-ttu-id="b3795-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b3795-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="b3795-157">Int32</span><span class="sxs-lookup"><span data-stu-id="b3795-157">Int32</span></span>|<span data-ttu-id="b3795-158">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="b3795-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="b3795-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b3795-159">errorDeviceCount</span></span>|<span data-ttu-id="b3795-160">Int32</span><span class="sxs-lookup"><span data-stu-id="b3795-160">Int32</span></span>|<span data-ttu-id="b3795-161">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="b3795-161">Number of error devices</span></span>|
|<span data-ttu-id="b3795-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b3795-162">conflictDeviceCount</span></span>|<span data-ttu-id="b3795-163">Int32</span><span class="sxs-lookup"><span data-stu-id="b3795-163">Int32</span></span>|<span data-ttu-id="b3795-164">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="b3795-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="b3795-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3795-165">Response</span></span>
<span data-ttu-id="b3795-166">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3795-166">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3795-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3795-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3795-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3795-168">Request</span></span>
<span data-ttu-id="b3795-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3795-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="b3795-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3795-170">Response</span></span>
<span data-ttu-id="b3795-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3795-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




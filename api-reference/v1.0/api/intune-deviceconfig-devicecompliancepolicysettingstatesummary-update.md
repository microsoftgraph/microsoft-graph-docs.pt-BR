---
title: Atualizar deviceCompliancePolicySettingStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicySettingStateSummary.
author: tfitzmac
ms.openlocfilehash: 87fb75ea6e0a059a83f17a06697131e6efa77a97
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351041"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="7743c-103">Atualizar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="7743c-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="7743c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7743c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7743c-105">Atualizar as propriedades de um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7743c-105">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7743c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7743c-106">Prerequisites</span></span>
<span data-ttu-id="7743c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7743c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7743c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7743c-109">Permission type</span></span>|<span data-ttu-id="7743c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7743c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7743c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7743c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7743c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7743c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7743c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7743c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7743c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7743c-114">Not supported.</span></span>|
|<span data-ttu-id="7743c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7743c-115">Application</span></span>|<span data-ttu-id="7743c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7743c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7743c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7743c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="7743c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7743c-118">Request headers</span></span>
|<span data-ttu-id="7743c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7743c-119">Header</span></span>|<span data-ttu-id="7743c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7743c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7743c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7743c-121">Authorization</span></span>|<span data-ttu-id="7743c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7743c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7743c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7743c-123">Accept</span></span>|<span data-ttu-id="7743c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7743c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7743c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7743c-125">Request body</span></span>
<span data-ttu-id="7743c-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7743c-126">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="7743c-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7743c-127">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="7743c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7743c-128">Property</span></span>|<span data-ttu-id="7743c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7743c-129">Type</span></span>|<span data-ttu-id="7743c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7743c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7743c-131">id</span><span class="sxs-lookup"><span data-stu-id="7743c-131">id</span></span>|<span data-ttu-id="7743c-132">String</span><span class="sxs-lookup"><span data-stu-id="7743c-132">String</span></span>|<span data-ttu-id="7743c-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7743c-133">Key of the entity.</span></span>|
|<span data-ttu-id="7743c-134">configuração</span><span class="sxs-lookup"><span data-stu-id="7743c-134">setting</span></span>|<span data-ttu-id="7743c-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7743c-135">String</span></span>|<span data-ttu-id="7743c-136">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="7743c-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="7743c-137">settingName</span><span class="sxs-lookup"><span data-stu-id="7743c-137">settingName</span></span>|<span data-ttu-id="7743c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7743c-138">String</span></span>|<span data-ttu-id="7743c-139">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="7743c-139">Name of the setting.</span></span>|
|<span data-ttu-id="7743c-140">platformType</span><span class="sxs-lookup"><span data-stu-id="7743c-140">platformType</span></span>|[<span data-ttu-id="7743c-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="7743c-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="7743c-142">Plataforma de configuração.</span><span class="sxs-lookup"><span data-stu-id="7743c-142">Setting platform.</span></span> <span data-ttu-id="7743c-143">Os valores possíveis são: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="7743c-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="7743c-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7743c-144">unknownDeviceCount</span></span>|<span data-ttu-id="7743c-145">Int32</span><span class="sxs-lookup"><span data-stu-id="7743c-145">Int32</span></span>|<span data-ttu-id="7743c-146">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="7743c-146">Number of unknown devices</span></span>|
|<span data-ttu-id="7743c-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7743c-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="7743c-148">Int32</span><span class="sxs-lookup"><span data-stu-id="7743c-148">Int32</span></span>|<span data-ttu-id="7743c-149">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="7743c-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="7743c-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7743c-150">compliantDeviceCount</span></span>|<span data-ttu-id="7743c-151">Int32</span><span class="sxs-lookup"><span data-stu-id="7743c-151">Int32</span></span>|<span data-ttu-id="7743c-152">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="7743c-152">Number of compliant devices</span></span>|
|<span data-ttu-id="7743c-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7743c-153">remediatedDeviceCount</span></span>|<span data-ttu-id="7743c-154">Int32</span><span class="sxs-lookup"><span data-stu-id="7743c-154">Int32</span></span>|<span data-ttu-id="7743c-155">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="7743c-155">Number of remediated devices</span></span>|
|<span data-ttu-id="7743c-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7743c-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="7743c-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7743c-157">Int32</span></span>|<span data-ttu-id="7743c-158">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="7743c-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="7743c-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7743c-159">errorDeviceCount</span></span>|<span data-ttu-id="7743c-160">Int32</span><span class="sxs-lookup"><span data-stu-id="7743c-160">Int32</span></span>|<span data-ttu-id="7743c-161">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="7743c-161">Number of error devices</span></span>|
|<span data-ttu-id="7743c-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7743c-162">conflictDeviceCount</span></span>|<span data-ttu-id="7743c-163">Int32</span><span class="sxs-lookup"><span data-stu-id="7743c-163">Int32</span></span>|<span data-ttu-id="7743c-164">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="7743c-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="7743c-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="7743c-165">Response</span></span>
<span data-ttu-id="7743c-166">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7743c-166">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7743c-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7743c-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="7743c-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7743c-168">Request</span></span>
<span data-ttu-id="7743c-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7743c-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7743c-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="7743c-170">Response</span></span>
<span data-ttu-id="7743c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7743c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




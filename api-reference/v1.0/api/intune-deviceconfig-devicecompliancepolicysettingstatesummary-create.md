---
title: Criar deviceCompliancePolicySettingStateSummary
description: Crie um novo objeto deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cf6fc766bfc54f452f9198dcbe3cee983b30f125
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980423"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="67a31-103">Criar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="67a31-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="67a31-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="67a31-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67a31-105">Crie um novo objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="67a31-105">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="67a31-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67a31-106">Prerequisites</span></span>
<span data-ttu-id="67a31-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67a31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67a31-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67a31-109">Permission type</span></span>|<span data-ttu-id="67a31-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67a31-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67a31-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67a31-111">Delegated (work or school account)</span></span>|<span data-ttu-id="67a31-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67a31-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="67a31-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67a31-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67a31-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67a31-114">Not supported.</span></span>|
|<span data-ttu-id="67a31-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67a31-115">Application</span></span>|<span data-ttu-id="67a31-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67a31-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67a31-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67a31-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="67a31-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67a31-118">Request headers</span></span>
|<span data-ttu-id="67a31-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67a31-119">Header</span></span>|<span data-ttu-id="67a31-120">Valor</span><span class="sxs-lookup"><span data-stu-id="67a31-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67a31-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="67a31-121">Authorization</span></span>|<span data-ttu-id="67a31-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67a31-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67a31-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67a31-123">Accept</span></span>|<span data-ttu-id="67a31-124">application/json</span><span class="sxs-lookup"><span data-stu-id="67a31-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67a31-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67a31-125">Request body</span></span>
<span data-ttu-id="67a31-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="67a31-126">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="67a31-127">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="67a31-127">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="67a31-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67a31-128">Property</span></span>|<span data-ttu-id="67a31-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="67a31-129">Type</span></span>|<span data-ttu-id="67a31-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="67a31-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67a31-131">id</span><span class="sxs-lookup"><span data-stu-id="67a31-131">id</span></span>|<span data-ttu-id="67a31-132">String</span><span class="sxs-lookup"><span data-stu-id="67a31-132">String</span></span>|<span data-ttu-id="67a31-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="67a31-133">Key of the entity.</span></span>|
|<span data-ttu-id="67a31-134">configuração</span><span class="sxs-lookup"><span data-stu-id="67a31-134">setting</span></span>|<span data-ttu-id="67a31-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67a31-135">String</span></span>|<span data-ttu-id="67a31-136">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="67a31-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="67a31-137">settingName</span><span class="sxs-lookup"><span data-stu-id="67a31-137">settingName</span></span>|<span data-ttu-id="67a31-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67a31-138">String</span></span>|<span data-ttu-id="67a31-139">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="67a31-139">Name of the setting.</span></span>|
|<span data-ttu-id="67a31-140">platformType</span><span class="sxs-lookup"><span data-stu-id="67a31-140">platformType</span></span>|[<span data-ttu-id="67a31-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="67a31-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="67a31-142">Plataforma de configuração.</span><span class="sxs-lookup"><span data-stu-id="67a31-142">Setting platform.</span></span> <span data-ttu-id="67a31-143">Os valores possíveis são: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="67a31-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="67a31-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="67a31-144">unknownDeviceCount</span></span>|<span data-ttu-id="67a31-145">Int32</span><span class="sxs-lookup"><span data-stu-id="67a31-145">Int32</span></span>|<span data-ttu-id="67a31-146">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="67a31-146">Number of unknown devices</span></span>|
|<span data-ttu-id="67a31-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="67a31-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="67a31-148">Int32</span><span class="sxs-lookup"><span data-stu-id="67a31-148">Int32</span></span>|<span data-ttu-id="67a31-149">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="67a31-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="67a31-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="67a31-150">compliantDeviceCount</span></span>|<span data-ttu-id="67a31-151">Int32</span><span class="sxs-lookup"><span data-stu-id="67a31-151">Int32</span></span>|<span data-ttu-id="67a31-152">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="67a31-152">Number of compliant devices</span></span>|
|<span data-ttu-id="67a31-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="67a31-153">remediatedDeviceCount</span></span>|<span data-ttu-id="67a31-154">Int32</span><span class="sxs-lookup"><span data-stu-id="67a31-154">Int32</span></span>|<span data-ttu-id="67a31-155">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="67a31-155">Number of remediated devices</span></span>|
|<span data-ttu-id="67a31-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="67a31-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="67a31-157">Int32</span><span class="sxs-lookup"><span data-stu-id="67a31-157">Int32</span></span>|<span data-ttu-id="67a31-158">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="67a31-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="67a31-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="67a31-159">errorDeviceCount</span></span>|<span data-ttu-id="67a31-160">Int32</span><span class="sxs-lookup"><span data-stu-id="67a31-160">Int32</span></span>|<span data-ttu-id="67a31-161">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="67a31-161">Number of error devices</span></span>|
|<span data-ttu-id="67a31-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="67a31-162">conflictDeviceCount</span></span>|<span data-ttu-id="67a31-163">Int32</span><span class="sxs-lookup"><span data-stu-id="67a31-163">Int32</span></span>|<span data-ttu-id="67a31-164">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="67a31-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="67a31-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="67a31-165">Response</span></span>
<span data-ttu-id="67a31-166">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67a31-166">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67a31-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67a31-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="67a31-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67a31-168">Request</span></span>
<span data-ttu-id="67a31-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67a31-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="67a31-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="67a31-170">Response</span></span>
<span data-ttu-id="67a31-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67a31-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




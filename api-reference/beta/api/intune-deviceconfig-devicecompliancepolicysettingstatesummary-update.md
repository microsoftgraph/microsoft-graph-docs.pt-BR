---
title: Atualizar deviceCompliancePolicySettingStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 80dc1770d2661a63e145e3f115465fffaef62490
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924122"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="a9904-103">Atualizar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="a9904-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="a9904-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a9904-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9904-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a9904-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9904-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a9904-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9904-107">Atualizar as propriedades de um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a9904-107">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a9904-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9904-108">Prerequisites</span></span>
<span data-ttu-id="a9904-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9904-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9904-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9904-111">Permission type</span></span>|<span data-ttu-id="a9904-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a9904-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9904-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9904-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9904-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9904-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9904-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9904-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9904-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9904-116">Not supported.</span></span>|
|<span data-ttu-id="a9904-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9904-117">Application</span></span>|<span data-ttu-id="a9904-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9904-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9904-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9904-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="a9904-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9904-120">Request headers</span></span>
|<span data-ttu-id="a9904-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9904-121">Header</span></span>|<span data-ttu-id="a9904-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a9904-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9904-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9904-123">Authorization</span></span>|<span data-ttu-id="a9904-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9904-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9904-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a9904-125">Accept</span></span>|<span data-ttu-id="a9904-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9904-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9904-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9904-127">Request body</span></span>
<span data-ttu-id="a9904-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a9904-128">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="a9904-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a9904-129">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="a9904-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9904-130">Property</span></span>|<span data-ttu-id="a9904-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9904-131">Type</span></span>|<span data-ttu-id="a9904-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9904-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9904-133">id</span><span class="sxs-lookup"><span data-stu-id="a9904-133">id</span></span>|<span data-ttu-id="a9904-134">String</span><span class="sxs-lookup"><span data-stu-id="a9904-134">String</span></span>|<span data-ttu-id="a9904-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a9904-135">Key of the entity.</span></span>|
|<span data-ttu-id="a9904-136">configuração</span><span class="sxs-lookup"><span data-stu-id="a9904-136">setting</span></span>|<span data-ttu-id="a9904-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9904-137">String</span></span>|<span data-ttu-id="a9904-138">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="a9904-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="a9904-139">settingName</span><span class="sxs-lookup"><span data-stu-id="a9904-139">settingName</span></span>|<span data-ttu-id="a9904-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9904-140">String</span></span>|<span data-ttu-id="a9904-141">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="a9904-141">Name of the setting.</span></span>|
|<span data-ttu-id="a9904-142">platformType</span><span class="sxs-lookup"><span data-stu-id="a9904-142">platformType</span></span>|[<span data-ttu-id="a9904-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="a9904-143">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="a9904-144">Plataforma de configuração.</span><span class="sxs-lookup"><span data-stu-id="a9904-144">Setting platform.</span></span> <span data-ttu-id="a9904-145">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="a9904-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="a9904-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a9904-146">unknownDeviceCount</span></span>|<span data-ttu-id="a9904-147">Int32</span><span class="sxs-lookup"><span data-stu-id="a9904-147">Int32</span></span>|<span data-ttu-id="a9904-148">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="a9904-148">Number of unknown devices</span></span>|
|<span data-ttu-id="a9904-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a9904-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="a9904-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a9904-150">Int32</span></span>|<span data-ttu-id="a9904-151">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="a9904-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="a9904-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a9904-152">compliantDeviceCount</span></span>|<span data-ttu-id="a9904-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a9904-153">Int32</span></span>|<span data-ttu-id="a9904-154">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="a9904-154">Number of compliant devices</span></span>|
|<span data-ttu-id="a9904-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a9904-155">remediatedDeviceCount</span></span>|<span data-ttu-id="a9904-156">Int32</span><span class="sxs-lookup"><span data-stu-id="a9904-156">Int32</span></span>|<span data-ttu-id="a9904-157">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="a9904-157">Number of remediated devices</span></span>|
|<span data-ttu-id="a9904-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a9904-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a9904-159">Int32</span><span class="sxs-lookup"><span data-stu-id="a9904-159">Int32</span></span>|<span data-ttu-id="a9904-160">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="a9904-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="a9904-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a9904-161">errorDeviceCount</span></span>|<span data-ttu-id="a9904-162">Int32</span><span class="sxs-lookup"><span data-stu-id="a9904-162">Int32</span></span>|<span data-ttu-id="a9904-163">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="a9904-163">Number of error devices</span></span>|
|<span data-ttu-id="a9904-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a9904-164">conflictDeviceCount</span></span>|<span data-ttu-id="a9904-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a9904-165">Int32</span></span>|<span data-ttu-id="a9904-166">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="a9904-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="a9904-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9904-167">Response</span></span>
<span data-ttu-id="a9904-168">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9904-168">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9904-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9904-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="a9904-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9904-170">Request</span></span>
<span data-ttu-id="a9904-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9904-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 322

{
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

### <a name="response"></a><span data-ttu-id="a9904-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9904-172">Response</span></span>
<span data-ttu-id="a9904-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9904-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






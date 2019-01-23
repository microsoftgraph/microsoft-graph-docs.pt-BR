---
title: Atualizar deviceCompliancePolicySettingStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicySettingStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 43aaa3b1269a6de2862ad15b8fda03eb92ec0631
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409773"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="bd488-103">Atualizar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="bd488-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="bd488-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="bd488-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bd488-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bd488-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd488-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="bd488-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd488-107">Atualizar as propriedades de um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="bd488-107">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd488-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bd488-108">Prerequisites</span></span>
<span data-ttu-id="bd488-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bd488-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bd488-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd488-111">Permission type</span></span>|<span data-ttu-id="bd488-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bd488-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd488-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd488-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd488-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd488-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bd488-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd488-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd488-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd488-116">Not supported.</span></span>|
|<span data-ttu-id="bd488-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd488-117">Application</span></span>|<span data-ttu-id="bd488-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd488-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd488-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd488-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="bd488-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd488-120">Request headers</span></span>
|<span data-ttu-id="bd488-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bd488-121">Header</span></span>|<span data-ttu-id="bd488-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bd488-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd488-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd488-123">Authorization</span></span>|<span data-ttu-id="bd488-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd488-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd488-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bd488-125">Accept</span></span>|<span data-ttu-id="bd488-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd488-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd488-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd488-127">Request body</span></span>
<span data-ttu-id="bd488-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="bd488-128">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="bd488-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="bd488-129">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="bd488-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd488-130">Property</span></span>|<span data-ttu-id="bd488-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd488-131">Type</span></span>|<span data-ttu-id="bd488-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd488-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd488-133">id</span><span class="sxs-lookup"><span data-stu-id="bd488-133">id</span></span>|<span data-ttu-id="bd488-134">String</span><span class="sxs-lookup"><span data-stu-id="bd488-134">String</span></span>|<span data-ttu-id="bd488-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bd488-135">Key of the entity.</span></span>|
|<span data-ttu-id="bd488-136">configuração</span><span class="sxs-lookup"><span data-stu-id="bd488-136">setting</span></span>|<span data-ttu-id="bd488-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd488-137">String</span></span>|<span data-ttu-id="bd488-138">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="bd488-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="bd488-139">settingName</span><span class="sxs-lookup"><span data-stu-id="bd488-139">settingName</span></span>|<span data-ttu-id="bd488-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd488-140">String</span></span>|<span data-ttu-id="bd488-141">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="bd488-141">Name of the setting.</span></span>|
|<span data-ttu-id="bd488-142">platformType</span><span class="sxs-lookup"><span data-stu-id="bd488-142">platformType</span></span>|[<span data-ttu-id="bd488-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="bd488-143">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="bd488-144">Plataforma de configuração.</span><span class="sxs-lookup"><span data-stu-id="bd488-144">Setting platform.</span></span> <span data-ttu-id="bd488-145">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="bd488-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="bd488-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd488-146">unknownDeviceCount</span></span>|<span data-ttu-id="bd488-147">Int32</span><span class="sxs-lookup"><span data-stu-id="bd488-147">Int32</span></span>|<span data-ttu-id="bd488-148">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="bd488-148">Number of unknown devices</span></span>|
|<span data-ttu-id="bd488-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd488-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="bd488-150">Int32</span><span class="sxs-lookup"><span data-stu-id="bd488-150">Int32</span></span>|<span data-ttu-id="bd488-151">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="bd488-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="bd488-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd488-152">compliantDeviceCount</span></span>|<span data-ttu-id="bd488-153">Int32</span><span class="sxs-lookup"><span data-stu-id="bd488-153">Int32</span></span>|<span data-ttu-id="bd488-154">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="bd488-154">Number of compliant devices</span></span>|
|<span data-ttu-id="bd488-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd488-155">remediatedDeviceCount</span></span>|<span data-ttu-id="bd488-156">Int32</span><span class="sxs-lookup"><span data-stu-id="bd488-156">Int32</span></span>|<span data-ttu-id="bd488-157">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="bd488-157">Number of remediated devices</span></span>|
|<span data-ttu-id="bd488-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd488-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="bd488-159">Int32</span><span class="sxs-lookup"><span data-stu-id="bd488-159">Int32</span></span>|<span data-ttu-id="bd488-160">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="bd488-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="bd488-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd488-161">errorDeviceCount</span></span>|<span data-ttu-id="bd488-162">Int32</span><span class="sxs-lookup"><span data-stu-id="bd488-162">Int32</span></span>|<span data-ttu-id="bd488-163">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="bd488-163">Number of error devices</span></span>|
|<span data-ttu-id="bd488-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd488-164">conflictDeviceCount</span></span>|<span data-ttu-id="bd488-165">Int32</span><span class="sxs-lookup"><span data-stu-id="bd488-165">Int32</span></span>|<span data-ttu-id="bd488-166">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="bd488-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="bd488-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd488-167">Response</span></span>
<span data-ttu-id="bd488-168">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd488-168">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd488-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd488-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd488-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd488-170">Request</span></span>
<span data-ttu-id="bd488-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd488-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bd488-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd488-172">Response</span></span>
<span data-ttu-id="bd488-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd488-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





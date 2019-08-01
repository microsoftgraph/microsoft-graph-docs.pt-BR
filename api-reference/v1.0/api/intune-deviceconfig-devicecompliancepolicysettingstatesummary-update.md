---
title: Atualizar deviceCompliancePolicySettingStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fdf5c66e2060a48003d55841cf92aae936561a65
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017753"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="6de23-103">Atualizar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="6de23-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="6de23-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6de23-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6de23-105">Atualizar as propriedades de um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6de23-105">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6de23-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6de23-106">Prerequisites</span></span>
<span data-ttu-id="6de23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6de23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6de23-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6de23-109">Permission type</span></span>|<span data-ttu-id="6de23-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6de23-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6de23-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6de23-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6de23-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6de23-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6de23-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6de23-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6de23-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6de23-114">Not supported.</span></span>|
|<span data-ttu-id="6de23-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6de23-115">Application</span></span>|<span data-ttu-id="6de23-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6de23-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6de23-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6de23-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="6de23-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6de23-118">Request headers</span></span>
|<span data-ttu-id="6de23-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6de23-119">Header</span></span>|<span data-ttu-id="6de23-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6de23-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6de23-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6de23-121">Authorization</span></span>|<span data-ttu-id="6de23-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6de23-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6de23-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6de23-123">Accept</span></span>|<span data-ttu-id="6de23-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6de23-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6de23-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6de23-125">Request body</span></span>
<span data-ttu-id="6de23-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6de23-126">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="6de23-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6de23-127">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="6de23-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6de23-128">Property</span></span>|<span data-ttu-id="6de23-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6de23-129">Type</span></span>|<span data-ttu-id="6de23-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6de23-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6de23-131">id</span><span class="sxs-lookup"><span data-stu-id="6de23-131">id</span></span>|<span data-ttu-id="6de23-132">String</span><span class="sxs-lookup"><span data-stu-id="6de23-132">String</span></span>|<span data-ttu-id="6de23-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6de23-133">Key of the entity.</span></span>|
|<span data-ttu-id="6de23-134">configuração</span><span class="sxs-lookup"><span data-stu-id="6de23-134">setting</span></span>|<span data-ttu-id="6de23-135">String</span><span class="sxs-lookup"><span data-stu-id="6de23-135">String</span></span>|<span data-ttu-id="6de23-136">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="6de23-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="6de23-137">settingName</span><span class="sxs-lookup"><span data-stu-id="6de23-137">settingName</span></span>|<span data-ttu-id="6de23-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6de23-138">String</span></span>|<span data-ttu-id="6de23-139">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="6de23-139">Name of the setting.</span></span>|
|<span data-ttu-id="6de23-140">platformType</span><span class="sxs-lookup"><span data-stu-id="6de23-140">platformType</span></span>|[<span data-ttu-id="6de23-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="6de23-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="6de23-142">Configuração de plataforma.</span><span class="sxs-lookup"><span data-stu-id="6de23-142">Setting platform.</span></span> <span data-ttu-id="6de23-143">Os valores possíveis são: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="6de23-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="6de23-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6de23-144">unknownDeviceCount</span></span>|<span data-ttu-id="6de23-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6de23-145">Int32</span></span>|<span data-ttu-id="6de23-146">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="6de23-146">Number of unknown devices</span></span>|
|<span data-ttu-id="6de23-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6de23-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="6de23-148">Int32</span><span class="sxs-lookup"><span data-stu-id="6de23-148">Int32</span></span>|<span data-ttu-id="6de23-149">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="6de23-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="6de23-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6de23-150">compliantDeviceCount</span></span>|<span data-ttu-id="6de23-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6de23-151">Int32</span></span>|<span data-ttu-id="6de23-152">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="6de23-152">Number of compliant devices</span></span>|
|<span data-ttu-id="6de23-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6de23-153">remediatedDeviceCount</span></span>|<span data-ttu-id="6de23-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6de23-154">Int32</span></span>|<span data-ttu-id="6de23-155">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="6de23-155">Number of remediated devices</span></span>|
|<span data-ttu-id="6de23-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6de23-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="6de23-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6de23-157">Int32</span></span>|<span data-ttu-id="6de23-158">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="6de23-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="6de23-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6de23-159">errorDeviceCount</span></span>|<span data-ttu-id="6de23-160">Int32</span><span class="sxs-lookup"><span data-stu-id="6de23-160">Int32</span></span>|<span data-ttu-id="6de23-161">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="6de23-161">Number of error devices</span></span>|
|<span data-ttu-id="6de23-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6de23-162">conflictDeviceCount</span></span>|<span data-ttu-id="6de23-163">Int32</span><span class="sxs-lookup"><span data-stu-id="6de23-163">Int32</span></span>|<span data-ttu-id="6de23-164">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="6de23-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="6de23-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="6de23-165">Response</span></span>
<span data-ttu-id="6de23-166">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6de23-166">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6de23-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6de23-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="6de23-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6de23-168">Request</span></span>
<span data-ttu-id="6de23-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6de23-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6de23-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="6de23-170">Response</span></span>
<span data-ttu-id="6de23-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6de23-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




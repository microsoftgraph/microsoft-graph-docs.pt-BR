---
title: Criar deviceCompliancePolicySettingStateSummary
description: Crie um novo objeto deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1bd0ab97129dda08db107e588c5c3103fbce2365
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975683"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="79b9e-103">Criar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="79b9e-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="79b9e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79b9e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79b9e-105">Crie um novo objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="79b9e-105">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79b9e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79b9e-106">Prerequisites</span></span>
<span data-ttu-id="79b9e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79b9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79b9e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79b9e-109">Permission type</span></span>|<span data-ttu-id="79b9e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="79b9e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79b9e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79b9e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="79b9e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79b9e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79b9e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79b9e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79b9e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79b9e-114">Not supported.</span></span>|
|<span data-ttu-id="79b9e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79b9e-115">Application</span></span>|<span data-ttu-id="79b9e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79b9e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79b9e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79b9e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="79b9e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79b9e-118">Request headers</span></span>
|<span data-ttu-id="79b9e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79b9e-119">Header</span></span>|<span data-ttu-id="79b9e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="79b9e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79b9e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="79b9e-121">Authorization</span></span>|<span data-ttu-id="79b9e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79b9e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79b9e-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79b9e-123">Accept</span></span>|<span data-ttu-id="79b9e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="79b9e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79b9e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79b9e-125">Request body</span></span>
<span data-ttu-id="79b9e-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="79b9e-126">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="79b9e-127">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="79b9e-127">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="79b9e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79b9e-128">Property</span></span>|<span data-ttu-id="79b9e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="79b9e-129">Type</span></span>|<span data-ttu-id="79b9e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="79b9e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79b9e-131">id</span><span class="sxs-lookup"><span data-stu-id="79b9e-131">id</span></span>|<span data-ttu-id="79b9e-132">String</span><span class="sxs-lookup"><span data-stu-id="79b9e-132">String</span></span>|<span data-ttu-id="79b9e-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="79b9e-133">Key of the entity.</span></span>|
|<span data-ttu-id="79b9e-134">configuração</span><span class="sxs-lookup"><span data-stu-id="79b9e-134">setting</span></span>|<span data-ttu-id="79b9e-135">String</span><span class="sxs-lookup"><span data-stu-id="79b9e-135">String</span></span>|<span data-ttu-id="79b9e-136">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="79b9e-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="79b9e-137">settingName</span><span class="sxs-lookup"><span data-stu-id="79b9e-137">settingName</span></span>|<span data-ttu-id="79b9e-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79b9e-138">String</span></span>|<span data-ttu-id="79b9e-139">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="79b9e-139">Name of the setting.</span></span>|
|<span data-ttu-id="79b9e-140">platformType</span><span class="sxs-lookup"><span data-stu-id="79b9e-140">platformType</span></span>|[<span data-ttu-id="79b9e-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="79b9e-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="79b9e-142">Configuração de plataforma.</span><span class="sxs-lookup"><span data-stu-id="79b9e-142">Setting platform.</span></span> <span data-ttu-id="79b9e-143">Os valores possíveis são: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="79b9e-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="79b9e-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="79b9e-144">unknownDeviceCount</span></span>|<span data-ttu-id="79b9e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="79b9e-145">Int32</span></span>|<span data-ttu-id="79b9e-146">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="79b9e-146">Number of unknown devices</span></span>|
|<span data-ttu-id="79b9e-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="79b9e-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="79b9e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="79b9e-148">Int32</span></span>|<span data-ttu-id="79b9e-149">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="79b9e-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="79b9e-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="79b9e-150">compliantDeviceCount</span></span>|<span data-ttu-id="79b9e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="79b9e-151">Int32</span></span>|<span data-ttu-id="79b9e-152">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="79b9e-152">Number of compliant devices</span></span>|
|<span data-ttu-id="79b9e-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="79b9e-153">remediatedDeviceCount</span></span>|<span data-ttu-id="79b9e-154">Int32</span><span class="sxs-lookup"><span data-stu-id="79b9e-154">Int32</span></span>|<span data-ttu-id="79b9e-155">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="79b9e-155">Number of remediated devices</span></span>|
|<span data-ttu-id="79b9e-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="79b9e-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="79b9e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="79b9e-157">Int32</span></span>|<span data-ttu-id="79b9e-158">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="79b9e-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="79b9e-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="79b9e-159">errorDeviceCount</span></span>|<span data-ttu-id="79b9e-160">Int32</span><span class="sxs-lookup"><span data-stu-id="79b9e-160">Int32</span></span>|<span data-ttu-id="79b9e-161">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="79b9e-161">Number of error devices</span></span>|
|<span data-ttu-id="79b9e-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="79b9e-162">conflictDeviceCount</span></span>|<span data-ttu-id="79b9e-163">Int32</span><span class="sxs-lookup"><span data-stu-id="79b9e-163">Int32</span></span>|<span data-ttu-id="79b9e-164">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="79b9e-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="79b9e-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="79b9e-165">Response</span></span>
<span data-ttu-id="79b9e-166">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79b9e-166">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79b9e-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79b9e-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="79b9e-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79b9e-168">Request</span></span>
<span data-ttu-id="79b9e-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79b9e-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="79b9e-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="79b9e-170">Response</span></span>
<span data-ttu-id="79b9e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79b9e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




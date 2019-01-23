---
title: Criar deviceCompliancePolicySettingStateSummary
description: Crie um novo objeto deviceCompliancePolicySettingStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 48bbae6e0252e7c0199d84802c71228ccbfebc04
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414183"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="ccc90-103">Criar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="ccc90-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="ccc90-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ccc90-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ccc90-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ccc90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ccc90-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ccc90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccc90-107">Crie um novo objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ccc90-107">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccc90-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ccc90-108">Prerequisites</span></span>
<span data-ttu-id="ccc90-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ccc90-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ccc90-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccc90-111">Permission type</span></span>|<span data-ttu-id="ccc90-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ccc90-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccc90-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccc90-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ccc90-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccc90-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ccc90-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccc90-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccc90-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccc90-116">Not supported.</span></span>|
|<span data-ttu-id="ccc90-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccc90-117">Application</span></span>|<span data-ttu-id="ccc90-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccc90-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccc90-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccc90-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="ccc90-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ccc90-120">Request headers</span></span>
|<span data-ttu-id="ccc90-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ccc90-121">Header</span></span>|<span data-ttu-id="ccc90-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ccc90-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccc90-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ccc90-123">Authorization</span></span>|<span data-ttu-id="ccc90-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccc90-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccc90-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ccc90-125">Accept</span></span>|<span data-ttu-id="ccc90-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ccc90-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccc90-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ccc90-127">Request body</span></span>
<span data-ttu-id="ccc90-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="ccc90-128">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="ccc90-129">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="ccc90-129">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="ccc90-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccc90-130">Property</span></span>|<span data-ttu-id="ccc90-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccc90-131">Type</span></span>|<span data-ttu-id="ccc90-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccc90-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccc90-133">id</span><span class="sxs-lookup"><span data-stu-id="ccc90-133">id</span></span>|<span data-ttu-id="ccc90-134">String</span><span class="sxs-lookup"><span data-stu-id="ccc90-134">String</span></span>|<span data-ttu-id="ccc90-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ccc90-135">Key of the entity.</span></span>|
|<span data-ttu-id="ccc90-136">configuração</span><span class="sxs-lookup"><span data-stu-id="ccc90-136">setting</span></span>|<span data-ttu-id="ccc90-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ccc90-137">String</span></span>|<span data-ttu-id="ccc90-138">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="ccc90-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="ccc90-139">settingName</span><span class="sxs-lookup"><span data-stu-id="ccc90-139">settingName</span></span>|<span data-ttu-id="ccc90-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ccc90-140">String</span></span>|<span data-ttu-id="ccc90-141">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="ccc90-141">Name of the setting.</span></span>|
|<span data-ttu-id="ccc90-142">platformType</span><span class="sxs-lookup"><span data-stu-id="ccc90-142">platformType</span></span>|[<span data-ttu-id="ccc90-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="ccc90-143">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="ccc90-144">Plataforma de configuração.</span><span class="sxs-lookup"><span data-stu-id="ccc90-144">Setting platform.</span></span> <span data-ttu-id="ccc90-145">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="ccc90-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="ccc90-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ccc90-146">unknownDeviceCount</span></span>|<span data-ttu-id="ccc90-147">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc90-147">Int32</span></span>|<span data-ttu-id="ccc90-148">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="ccc90-148">Number of unknown devices</span></span>|
|<span data-ttu-id="ccc90-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ccc90-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="ccc90-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc90-150">Int32</span></span>|<span data-ttu-id="ccc90-151">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="ccc90-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="ccc90-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ccc90-152">compliantDeviceCount</span></span>|<span data-ttu-id="ccc90-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc90-153">Int32</span></span>|<span data-ttu-id="ccc90-154">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="ccc90-154">Number of compliant devices</span></span>|
|<span data-ttu-id="ccc90-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ccc90-155">remediatedDeviceCount</span></span>|<span data-ttu-id="ccc90-156">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc90-156">Int32</span></span>|<span data-ttu-id="ccc90-157">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="ccc90-157">Number of remediated devices</span></span>|
|<span data-ttu-id="ccc90-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ccc90-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="ccc90-159">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc90-159">Int32</span></span>|<span data-ttu-id="ccc90-160">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="ccc90-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="ccc90-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ccc90-161">errorDeviceCount</span></span>|<span data-ttu-id="ccc90-162">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc90-162">Int32</span></span>|<span data-ttu-id="ccc90-163">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="ccc90-163">Number of error devices</span></span>|
|<span data-ttu-id="ccc90-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ccc90-164">conflictDeviceCount</span></span>|<span data-ttu-id="ccc90-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc90-165">Int32</span></span>|<span data-ttu-id="ccc90-166">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="ccc90-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="ccc90-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccc90-167">Response</span></span>
<span data-ttu-id="ccc90-168">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccc90-168">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccc90-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ccc90-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccc90-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccc90-170">Request</span></span>
<span data-ttu-id="ccc90-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccc90-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="ccc90-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccc90-172">Response</span></span>
<span data-ttu-id="ccc90-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ccc90-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





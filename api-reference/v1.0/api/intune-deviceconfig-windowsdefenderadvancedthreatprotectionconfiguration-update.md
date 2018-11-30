---
title: Atualizar windowsDefenderAdvancedThreatProtectionConfiguration
description: Atualizar as propriedades de um objeto windowsDefenderAdvancedThreatProtectionConfiguration.
ms.openlocfilehash: 59fca8540c5c2f5e499f709c2a4547274fde800f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005060"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="5becf-103">Atualizar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="5becf-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="5becf-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5becf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5becf-105">Atualizar as propriedades de um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5becf-105">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5becf-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5becf-106">Prerequisites</span></span>
<span data-ttu-id="5becf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5becf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5becf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5becf-109">Permission type</span></span>|<span data-ttu-id="5becf-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5becf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5becf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5becf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5becf-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5becf-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5becf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5becf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5becf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5becf-114">Not supported.</span></span>|
|<span data-ttu-id="5becf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5becf-115">Application</span></span>|<span data-ttu-id="5becf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5becf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5becf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5becf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5becf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5becf-118">Request headers</span></span>
|<span data-ttu-id="5becf-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5becf-119">Header</span></span>|<span data-ttu-id="5becf-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5becf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5becf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5becf-121">Authorization</span></span>|<span data-ttu-id="5becf-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5becf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5becf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5becf-123">Accept</span></span>|<span data-ttu-id="5becf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5becf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5becf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5becf-125">Request body</span></span>
<span data-ttu-id="5becf-126">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5becf-126">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="5becf-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5becf-127">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="5becf-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5becf-128">Property</span></span>|<span data-ttu-id="5becf-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="5becf-129">Type</span></span>|<span data-ttu-id="5becf-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="5becf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5becf-131">id</span><span class="sxs-lookup"><span data-stu-id="5becf-131">id</span></span>|<span data-ttu-id="5becf-132">String</span><span class="sxs-lookup"><span data-stu-id="5becf-132">String</span></span>|<span data-ttu-id="5becf-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5becf-133">Key of the entity.</span></span> <span data-ttu-id="5becf-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5becf-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5becf-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5becf-135">lastModifiedDateTime</span></span>|<span data-ttu-id="5becf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5becf-136">DateTimeOffset</span></span>|<span data-ttu-id="5becf-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5becf-137">DateTime the object was last modified.</span></span> <span data-ttu-id="5becf-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5becf-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5becf-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5becf-139">createdDateTime</span></span>|<span data-ttu-id="5becf-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5becf-140">DateTimeOffset</span></span>|<span data-ttu-id="5becf-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5becf-141">DateTime the object was created.</span></span> <span data-ttu-id="5becf-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5becf-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5becf-143">description</span><span class="sxs-lookup"><span data-stu-id="5becf-143">description</span></span>|<span data-ttu-id="5becf-144">String</span><span class="sxs-lookup"><span data-stu-id="5becf-144">String</span></span>|<span data-ttu-id="5becf-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5becf-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5becf-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5becf-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5becf-147">displayName</span><span class="sxs-lookup"><span data-stu-id="5becf-147">displayName</span></span>|<span data-ttu-id="5becf-148">String</span><span class="sxs-lookup"><span data-stu-id="5becf-148">String</span></span>|<span data-ttu-id="5becf-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5becf-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5becf-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5becf-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5becf-151">version</span><span class="sxs-lookup"><span data-stu-id="5becf-151">version</span></span>|<span data-ttu-id="5becf-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5becf-152">Int32</span></span>|<span data-ttu-id="5becf-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5becf-153">Version of the device configuration.</span></span> <span data-ttu-id="5becf-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5becf-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5becf-155">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="5becf-155">allowSampleSharing</span></span>|<span data-ttu-id="5becf-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="5becf-156">Boolean</span></span>|<span data-ttu-id="5becf-157">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="5becf-157">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="5becf-158">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="5becf-158">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="5becf-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="5becf-159">Boolean</span></span>|<span data-ttu-id="5becf-160">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="5becf-160">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="5becf-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="5becf-161">Response</span></span>
<span data-ttu-id="5becf-162">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5becf-162">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5becf-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5becf-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="5becf-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5becf-164">Request</span></span>
<span data-ttu-id="5becf-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5becf-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 267

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```

### <a name="response"></a><span data-ttu-id="5becf-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="5becf-166">Response</span></span>
<span data-ttu-id="5becf-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5becf-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```




---
title: Criar windowsDefenderAdvancedThreatProtectionConfiguration
description: Criar um novo objeto windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 073301ce6e00bc7d33926468158feb39c8ac67d4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844447"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="1e07b-103">Criar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="1e07b-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="1e07b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1e07b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e07b-105">Criar um novo objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e07b-105">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e07b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e07b-106">Prerequisites</span></span>
<span data-ttu-id="1e07b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e07b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e07b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e07b-109">Permission type</span></span>|<span data-ttu-id="1e07b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e07b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e07b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e07b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1e07b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e07b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1e07b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e07b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e07b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e07b-114">Not supported.</span></span>|
|<span data-ttu-id="1e07b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e07b-115">Application</span></span>|<span data-ttu-id="1e07b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e07b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e07b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e07b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1e07b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e07b-118">Request headers</span></span>
|<span data-ttu-id="1e07b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e07b-119">Header</span></span>|<span data-ttu-id="1e07b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1e07b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e07b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e07b-121">Authorization</span></span>|<span data-ttu-id="1e07b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e07b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e07b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e07b-123">Accept</span></span>|<span data-ttu-id="1e07b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1e07b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e07b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e07b-125">Request body</span></span>
<span data-ttu-id="1e07b-126">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1e07b-126">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="1e07b-127">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1e07b-127">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="1e07b-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e07b-128">Property</span></span>|<span data-ttu-id="1e07b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e07b-129">Type</span></span>|<span data-ttu-id="1e07b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e07b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e07b-131">id</span><span class="sxs-lookup"><span data-stu-id="1e07b-131">id</span></span>|<span data-ttu-id="1e07b-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e07b-132">String</span></span>|<span data-ttu-id="1e07b-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1e07b-133">Key of the entity.</span></span> <span data-ttu-id="1e07b-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e07b-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e07b-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e07b-135">lastModifiedDateTime</span></span>|<span data-ttu-id="1e07b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e07b-136">DateTimeOffset</span></span>|<span data-ttu-id="1e07b-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1e07b-137">DateTime the object was last modified.</span></span> <span data-ttu-id="1e07b-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e07b-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e07b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e07b-139">createdDateTime</span></span>|<span data-ttu-id="1e07b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e07b-140">DateTimeOffset</span></span>|<span data-ttu-id="1e07b-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1e07b-141">DateTime the object was created.</span></span> <span data-ttu-id="1e07b-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e07b-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e07b-143">description</span><span class="sxs-lookup"><span data-stu-id="1e07b-143">description</span></span>|<span data-ttu-id="1e07b-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e07b-144">String</span></span>|<span data-ttu-id="1e07b-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e07b-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1e07b-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e07b-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e07b-147">displayName</span><span class="sxs-lookup"><span data-stu-id="1e07b-147">displayName</span></span>|<span data-ttu-id="1e07b-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e07b-148">String</span></span>|<span data-ttu-id="1e07b-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e07b-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1e07b-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e07b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e07b-151">version</span><span class="sxs-lookup"><span data-stu-id="1e07b-151">version</span></span>|<span data-ttu-id="1e07b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1e07b-152">Int32</span></span>|<span data-ttu-id="1e07b-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e07b-153">Version of the device configuration.</span></span> <span data-ttu-id="1e07b-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e07b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e07b-155">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="1e07b-155">allowSampleSharing</span></span>|<span data-ttu-id="1e07b-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e07b-156">Boolean</span></span>|<span data-ttu-id="1e07b-157">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="1e07b-157">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="1e07b-158">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="1e07b-158">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="1e07b-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e07b-159">Boolean</span></span>|<span data-ttu-id="1e07b-160">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="1e07b-160">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="1e07b-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e07b-161">Response</span></span>
<span data-ttu-id="1e07b-162">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e07b-162">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e07b-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e07b-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e07b-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e07b-164">Request</span></span>
<span data-ttu-id="1e07b-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e07b-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="1e07b-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e07b-166">Response</span></span>
<span data-ttu-id="1e07b-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e07b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




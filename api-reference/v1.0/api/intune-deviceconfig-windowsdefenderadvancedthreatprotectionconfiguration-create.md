---
title: Criar windowsDefenderAdvancedThreatProtectionConfiguration
description: Criar um novo objeto windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 54c540192a9f46b7a5857dbcc0344fcfd298cce0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932753"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="8215e-103">Criar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="8215e-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="8215e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8215e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8215e-105">Criar um novo objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8215e-105">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8215e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8215e-106">Prerequisites</span></span>
<span data-ttu-id="8215e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8215e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8215e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8215e-109">Permission type</span></span>|<span data-ttu-id="8215e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8215e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8215e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8215e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8215e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8215e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8215e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8215e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8215e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8215e-114">Not supported.</span></span>|
|<span data-ttu-id="8215e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8215e-115">Application</span></span>|<span data-ttu-id="8215e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8215e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8215e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8215e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8215e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8215e-118">Request headers</span></span>
|<span data-ttu-id="8215e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8215e-119">Header</span></span>|<span data-ttu-id="8215e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8215e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8215e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8215e-121">Authorization</span></span>|<span data-ttu-id="8215e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8215e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8215e-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8215e-123">Accept</span></span>|<span data-ttu-id="8215e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8215e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8215e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8215e-125">Request body</span></span>
<span data-ttu-id="8215e-126">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8215e-126">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="8215e-127">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8215e-127">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="8215e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8215e-128">Property</span></span>|<span data-ttu-id="8215e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8215e-129">Type</span></span>|<span data-ttu-id="8215e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8215e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8215e-131">id</span><span class="sxs-lookup"><span data-stu-id="8215e-131">id</span></span>|<span data-ttu-id="8215e-132">String</span><span class="sxs-lookup"><span data-stu-id="8215e-132">String</span></span>|<span data-ttu-id="8215e-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8215e-133">Key of the entity.</span></span> <span data-ttu-id="8215e-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8215e-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8215e-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8215e-135">lastModifiedDateTime</span></span>|<span data-ttu-id="8215e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8215e-136">DateTimeOffset</span></span>|<span data-ttu-id="8215e-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8215e-137">DateTime the object was last modified.</span></span> <span data-ttu-id="8215e-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8215e-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8215e-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8215e-139">createdDateTime</span></span>|<span data-ttu-id="8215e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8215e-140">DateTimeOffset</span></span>|<span data-ttu-id="8215e-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8215e-141">DateTime the object was created.</span></span> <span data-ttu-id="8215e-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8215e-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8215e-143">description</span><span class="sxs-lookup"><span data-stu-id="8215e-143">description</span></span>|<span data-ttu-id="8215e-144">String</span><span class="sxs-lookup"><span data-stu-id="8215e-144">String</span></span>|<span data-ttu-id="8215e-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8215e-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8215e-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8215e-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8215e-147">displayName</span><span class="sxs-lookup"><span data-stu-id="8215e-147">displayName</span></span>|<span data-ttu-id="8215e-148">String</span><span class="sxs-lookup"><span data-stu-id="8215e-148">String</span></span>|<span data-ttu-id="8215e-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8215e-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8215e-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8215e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8215e-151">version</span><span class="sxs-lookup"><span data-stu-id="8215e-151">version</span></span>|<span data-ttu-id="8215e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8215e-152">Int32</span></span>|<span data-ttu-id="8215e-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8215e-153">Version of the device configuration.</span></span> <span data-ttu-id="8215e-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8215e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8215e-155">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="8215e-155">allowSampleSharing</span></span>|<span data-ttu-id="8215e-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="8215e-156">Boolean</span></span>|<span data-ttu-id="8215e-157">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="8215e-157">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="8215e-158">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="8215e-158">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="8215e-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="8215e-159">Boolean</span></span>|<span data-ttu-id="8215e-160">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="8215e-160">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="8215e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="8215e-161">Response</span></span>
<span data-ttu-id="8215e-162">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8215e-162">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8215e-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8215e-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="8215e-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8215e-164">Request</span></span>
<span data-ttu-id="8215e-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8215e-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8215e-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="8215e-166">Response</span></span>
<span data-ttu-id="8215e-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8215e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




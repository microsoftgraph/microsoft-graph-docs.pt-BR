---
title: Atualizar windowsDefenderAdvancedThreatProtectionConfiguration
description: Atualizar as propriedades de um objeto windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9444397e61ee64a056600b77afac8cf7b1075e3b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997082"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="71a1c-103">Atualizar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="71a1c-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="71a1c-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71a1c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71a1c-105">Atualizar as propriedades de um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71a1c-105">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71a1c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71a1c-106">Prerequisites</span></span>
<span data-ttu-id="71a1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71a1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71a1c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71a1c-109">Permission type</span></span>|<span data-ttu-id="71a1c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="71a1c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71a1c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71a1c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="71a1c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71a1c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71a1c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71a1c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71a1c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71a1c-114">Not supported.</span></span>|
|<span data-ttu-id="71a1c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71a1c-115">Application</span></span>|<span data-ttu-id="71a1c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71a1c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71a1c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71a1c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="71a1c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71a1c-118">Request headers</span></span>
|<span data-ttu-id="71a1c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71a1c-119">Header</span></span>|<span data-ttu-id="71a1c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="71a1c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71a1c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="71a1c-121">Authorization</span></span>|<span data-ttu-id="71a1c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71a1c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71a1c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71a1c-123">Accept</span></span>|<span data-ttu-id="71a1c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="71a1c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71a1c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71a1c-125">Request body</span></span>
<span data-ttu-id="71a1c-126">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71a1c-126">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="71a1c-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71a1c-127">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="71a1c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71a1c-128">Property</span></span>|<span data-ttu-id="71a1c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="71a1c-129">Type</span></span>|<span data-ttu-id="71a1c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="71a1c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71a1c-131">id</span><span class="sxs-lookup"><span data-stu-id="71a1c-131">id</span></span>|<span data-ttu-id="71a1c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71a1c-132">String</span></span>|<span data-ttu-id="71a1c-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="71a1c-133">Key of the entity.</span></span> <span data-ttu-id="71a1c-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71a1c-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71a1c-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71a1c-135">lastModifiedDateTime</span></span>|<span data-ttu-id="71a1c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71a1c-136">DateTimeOffset</span></span>|<span data-ttu-id="71a1c-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="71a1c-137">DateTime the object was last modified.</span></span> <span data-ttu-id="71a1c-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71a1c-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71a1c-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71a1c-139">createdDateTime</span></span>|<span data-ttu-id="71a1c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71a1c-140">DateTimeOffset</span></span>|<span data-ttu-id="71a1c-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="71a1c-141">DateTime the object was created.</span></span> <span data-ttu-id="71a1c-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71a1c-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71a1c-143">descrição</span><span class="sxs-lookup"><span data-stu-id="71a1c-143">description</span></span>|<span data-ttu-id="71a1c-144">String</span><span class="sxs-lookup"><span data-stu-id="71a1c-144">String</span></span>|<span data-ttu-id="71a1c-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="71a1c-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="71a1c-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71a1c-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71a1c-147">displayName</span><span class="sxs-lookup"><span data-stu-id="71a1c-147">displayName</span></span>|<span data-ttu-id="71a1c-148">String</span><span class="sxs-lookup"><span data-stu-id="71a1c-148">String</span></span>|<span data-ttu-id="71a1c-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="71a1c-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="71a1c-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71a1c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71a1c-151">versão</span><span class="sxs-lookup"><span data-stu-id="71a1c-151">version</span></span>|<span data-ttu-id="71a1c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="71a1c-152">Int32</span></span>|<span data-ttu-id="71a1c-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="71a1c-153">Version of the device configuration.</span></span> <span data-ttu-id="71a1c-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71a1c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71a1c-155">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="71a1c-155">allowSampleSharing</span></span>|<span data-ttu-id="71a1c-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="71a1c-156">Boolean</span></span>|<span data-ttu-id="71a1c-157">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="71a1c-157">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="71a1c-158">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="71a1c-158">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="71a1c-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="71a1c-159">Boolean</span></span>|<span data-ttu-id="71a1c-160">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="71a1c-160">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="71a1c-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="71a1c-161">Response</span></span>
<span data-ttu-id="71a1c-162">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71a1c-162">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71a1c-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71a1c-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="71a1c-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71a1c-164">Request</span></span>
<span data-ttu-id="71a1c-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71a1c-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="71a1c-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="71a1c-166">Response</span></span>
<span data-ttu-id="71a1c-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71a1c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




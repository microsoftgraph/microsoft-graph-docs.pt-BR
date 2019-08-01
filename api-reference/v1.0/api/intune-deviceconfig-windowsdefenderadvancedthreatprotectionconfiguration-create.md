---
title: Criar windowsDefenderAdvancedThreatProtectionConfiguration
description: Criar um novo objeto windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a762ae3697166efbac3680c8f92dba12bde68b43
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997103"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="9f304-103">Criar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="9f304-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="9f304-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9f304-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f304-105">Criar um novo objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f304-105">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f304-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9f304-106">Prerequisites</span></span>
<span data-ttu-id="9f304-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f304-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f304-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f304-109">Permission type</span></span>|<span data-ttu-id="9f304-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9f304-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f304-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f304-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9f304-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f304-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f304-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f304-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f304-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f304-114">Not supported.</span></span>|
|<span data-ttu-id="9f304-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f304-115">Application</span></span>|<span data-ttu-id="9f304-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f304-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f304-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f304-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9f304-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f304-118">Request headers</span></span>
|<span data-ttu-id="9f304-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9f304-119">Header</span></span>|<span data-ttu-id="9f304-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9f304-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f304-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f304-121">Authorization</span></span>|<span data-ttu-id="9f304-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f304-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f304-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9f304-123">Accept</span></span>|<span data-ttu-id="9f304-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9f304-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f304-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f304-125">Request body</span></span>
<span data-ttu-id="9f304-126">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9f304-126">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="9f304-127">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9f304-127">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="9f304-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f304-128">Property</span></span>|<span data-ttu-id="9f304-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f304-129">Type</span></span>|<span data-ttu-id="9f304-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f304-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f304-131">id</span><span class="sxs-lookup"><span data-stu-id="9f304-131">id</span></span>|<span data-ttu-id="9f304-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f304-132">String</span></span>|<span data-ttu-id="9f304-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9f304-133">Key of the entity.</span></span> <span data-ttu-id="9f304-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f304-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f304-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f304-135">lastModifiedDateTime</span></span>|<span data-ttu-id="9f304-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f304-136">DateTimeOffset</span></span>|<span data-ttu-id="9f304-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9f304-137">DateTime the object was last modified.</span></span> <span data-ttu-id="9f304-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f304-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f304-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f304-139">createdDateTime</span></span>|<span data-ttu-id="9f304-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f304-140">DateTimeOffset</span></span>|<span data-ttu-id="9f304-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9f304-141">DateTime the object was created.</span></span> <span data-ttu-id="9f304-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f304-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f304-143">descrição</span><span class="sxs-lookup"><span data-stu-id="9f304-143">description</span></span>|<span data-ttu-id="9f304-144">String</span><span class="sxs-lookup"><span data-stu-id="9f304-144">String</span></span>|<span data-ttu-id="9f304-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9f304-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9f304-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f304-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f304-147">displayName</span><span class="sxs-lookup"><span data-stu-id="9f304-147">displayName</span></span>|<span data-ttu-id="9f304-148">String</span><span class="sxs-lookup"><span data-stu-id="9f304-148">String</span></span>|<span data-ttu-id="9f304-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9f304-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9f304-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f304-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f304-151">versão</span><span class="sxs-lookup"><span data-stu-id="9f304-151">version</span></span>|<span data-ttu-id="9f304-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9f304-152">Int32</span></span>|<span data-ttu-id="9f304-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9f304-153">Version of the device configuration.</span></span> <span data-ttu-id="9f304-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f304-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f304-155">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="9f304-155">allowSampleSharing</span></span>|<span data-ttu-id="9f304-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="9f304-156">Boolean</span></span>|<span data-ttu-id="9f304-157">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="9f304-157">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="9f304-158">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="9f304-158">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="9f304-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="9f304-159">Boolean</span></span>|<span data-ttu-id="9f304-160">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="9f304-160">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="9f304-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f304-161">Response</span></span>
<span data-ttu-id="9f304-162">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f304-162">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f304-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f304-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f304-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f304-164">Request</span></span>
<span data-ttu-id="9f304-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f304-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f304-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f304-166">Response</span></span>
<span data-ttu-id="9f304-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f304-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




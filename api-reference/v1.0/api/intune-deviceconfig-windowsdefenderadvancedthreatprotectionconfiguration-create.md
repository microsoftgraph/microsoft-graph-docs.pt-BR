---
title: Criar windowsDefenderAdvancedThreatProtectionConfiguration
description: Criar um novo objeto windowsDefenderAdvancedThreatProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 69beca8d20c1c3bda2faae24f9e44374eb4e9e5e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069929"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="ffa8f-103">Criar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="ffa8f-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

<span data-ttu-id="ffa8f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffa8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ffa8f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ffa8f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffa8f-106">Criar um novo objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffa8f-106">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffa8f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ffa8f-107">Prerequisites</span></span>
<span data-ttu-id="ffa8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffa8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffa8f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ffa8f-110">Permission type</span></span>|<span data-ttu-id="ffa8f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ffa8f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffa8f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ffa8f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ffa8f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffa8f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ffa8f-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ffa8f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffa8f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ffa8f-115">Not supported.</span></span>|
|<span data-ttu-id="ffa8f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ffa8f-116">Application</span></span>|<span data-ttu-id="ffa8f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ffa8f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffa8f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ffa8f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ffa8f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ffa8f-119">Request headers</span></span>
|<span data-ttu-id="ffa8f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ffa8f-120">Header</span></span>|<span data-ttu-id="ffa8f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ffa8f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffa8f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ffa8f-122">Authorization</span></span>|<span data-ttu-id="ffa8f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ffa8f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffa8f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ffa8f-124">Accept</span></span>|<span data-ttu-id="ffa8f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ffa8f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffa8f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ffa8f-126">Request body</span></span>
<span data-ttu-id="ffa8f-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ffa8f-127">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="ffa8f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ffa8f-128">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="ffa8f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ffa8f-129">Property</span></span>|<span data-ttu-id="ffa8f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffa8f-130">Type</span></span>|<span data-ttu-id="ffa8f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffa8f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffa8f-132">id</span><span class="sxs-lookup"><span data-stu-id="ffa8f-132">id</span></span>|<span data-ttu-id="ffa8f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ffa8f-133">String</span></span>|<span data-ttu-id="ffa8f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ffa8f-134">Key of the entity.</span></span> <span data-ttu-id="ffa8f-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffa8f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffa8f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ffa8f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ffa8f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffa8f-137">DateTimeOffset</span></span>|<span data-ttu-id="ffa8f-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ffa8f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ffa8f-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffa8f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffa8f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffa8f-140">createdDateTime</span></span>|<span data-ttu-id="ffa8f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffa8f-141">DateTimeOffset</span></span>|<span data-ttu-id="ffa8f-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ffa8f-142">DateTime the object was created.</span></span> <span data-ttu-id="ffa8f-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffa8f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffa8f-144">description</span><span class="sxs-lookup"><span data-stu-id="ffa8f-144">description</span></span>|<span data-ttu-id="ffa8f-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ffa8f-145">String</span></span>|<span data-ttu-id="ffa8f-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ffa8f-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ffa8f-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffa8f-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffa8f-148">displayName</span><span class="sxs-lookup"><span data-stu-id="ffa8f-148">displayName</span></span>|<span data-ttu-id="ffa8f-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ffa8f-149">String</span></span>|<span data-ttu-id="ffa8f-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ffa8f-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ffa8f-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffa8f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffa8f-152">versão</span><span class="sxs-lookup"><span data-stu-id="ffa8f-152">version</span></span>|<span data-ttu-id="ffa8f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ffa8f-153">Int32</span></span>|<span data-ttu-id="ffa8f-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ffa8f-154">Version of the device configuration.</span></span> <span data-ttu-id="ffa8f-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffa8f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffa8f-156">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="ffa8f-156">allowSampleSharing</span></span>|<span data-ttu-id="ffa8f-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffa8f-157">Boolean</span></span>|<span data-ttu-id="ffa8f-158">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="ffa8f-158">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="ffa8f-159">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="ffa8f-159">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="ffa8f-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffa8f-160">Boolean</span></span>|<span data-ttu-id="ffa8f-161">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="ffa8f-161">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="ffa8f-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffa8f-162">Response</span></span>
<span data-ttu-id="ffa8f-163">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ffa8f-163">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffa8f-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ffa8f-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffa8f-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ffa8f-165">Request</span></span>
<span data-ttu-id="ffa8f-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ffa8f-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ffa8f-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffa8f-167">Response</span></span>
<span data-ttu-id="ffa8f-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ffa8f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










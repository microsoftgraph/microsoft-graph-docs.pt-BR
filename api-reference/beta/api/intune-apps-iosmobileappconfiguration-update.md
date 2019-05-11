---
title: Atualizar iosMobileAppConfiguration
description: Atualiza as propriedades de um objeto iosMobileAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ec86cfbfb671789ed67f154d230559e02a9df63
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33936879"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="6d2fb-103">Atualizar iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6d2fb-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="6d2fb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d2fb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d2fb-106">Atualiza as propriedades de um objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d2fb-106">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d2fb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6d2fb-107">Prerequisites</span></span>
<span data-ttu-id="6d2fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d2fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d2fb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d2fb-110">Permission type</span></span>|<span data-ttu-id="6d2fb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6d2fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d2fb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d2fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6d2fb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d2fb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6d2fb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d2fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d2fb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-115">Not supported.</span></span>|
|<span data-ttu-id="6d2fb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d2fb-116">Application</span></span>|<span data-ttu-id="6d2fb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d2fb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d2fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6d2fb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d2fb-119">Request headers</span></span>
|<span data-ttu-id="6d2fb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d2fb-120">Header</span></span>|<span data-ttu-id="6d2fb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6d2fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d2fb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d2fb-122">Authorization</span></span>|<span data-ttu-id="6d2fb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d2fb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d2fb-124">Accept</span></span>|<span data-ttu-id="6d2fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6d2fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d2fb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d2fb-126">Request body</span></span>
<span data-ttu-id="6d2fb-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d2fb-127">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="6d2fb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d2fb-128">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="6d2fb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d2fb-129">Property</span></span>|<span data-ttu-id="6d2fb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d2fb-130">Type</span></span>|<span data-ttu-id="6d2fb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d2fb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d2fb-132">id</span><span class="sxs-lookup"><span data-stu-id="6d2fb-132">id</span></span>|<span data-ttu-id="6d2fb-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d2fb-133">String</span></span>|<span data-ttu-id="6d2fb-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-134">Key of the entity.</span></span> <span data-ttu-id="6d2fb-135">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d2fb-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6d2fb-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="6d2fb-136">targetedMobileApps</span></span>|<span data-ttu-id="6d2fb-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d2fb-137">String collection</span></span>|<span data-ttu-id="6d2fb-138">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-138">the associated app.</span></span> <span data-ttu-id="6d2fb-139">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d2fb-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6d2fb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6d2fb-140">roleScopeTagIds</span></span>|<span data-ttu-id="6d2fb-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d2fb-141">String collection</span></span>|<span data-ttu-id="6d2fb-142">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="6d2fb-143">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d2fb-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6d2fb-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d2fb-144">createdDateTime</span></span>|<span data-ttu-id="6d2fb-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d2fb-145">DateTimeOffset</span></span>|<span data-ttu-id="6d2fb-146">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-146">DateTime the object was created.</span></span> <span data-ttu-id="6d2fb-147">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d2fb-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6d2fb-148">description</span><span class="sxs-lookup"><span data-stu-id="6d2fb-148">description</span></span>|<span data-ttu-id="6d2fb-149">String</span><span class="sxs-lookup"><span data-stu-id="6d2fb-149">String</span></span>|<span data-ttu-id="6d2fb-150">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6d2fb-151">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d2fb-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6d2fb-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d2fb-152">lastModifiedDateTime</span></span>|<span data-ttu-id="6d2fb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d2fb-153">DateTimeOffset</span></span>|<span data-ttu-id="6d2fb-154">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-154">DateTime the object was last modified.</span></span> <span data-ttu-id="6d2fb-155">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d2fb-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6d2fb-156">displayName</span><span class="sxs-lookup"><span data-stu-id="6d2fb-156">displayName</span></span>|<span data-ttu-id="6d2fb-157">String</span><span class="sxs-lookup"><span data-stu-id="6d2fb-157">String</span></span>|<span data-ttu-id="6d2fb-158">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6d2fb-159">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d2fb-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6d2fb-160">version</span><span class="sxs-lookup"><span data-stu-id="6d2fb-160">version</span></span>|<span data-ttu-id="6d2fb-161">Int32</span><span class="sxs-lookup"><span data-stu-id="6d2fb-161">Int32</span></span>|<span data-ttu-id="6d2fb-162">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-162">Version of the device configuration.</span></span> <span data-ttu-id="6d2fb-163">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d2fb-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6d2fb-164">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="6d2fb-164">encodedSettingXml</span></span>|<span data-ttu-id="6d2fb-165">Binária</span><span class="sxs-lookup"><span data-stu-id="6d2fb-165">Binary</span></span>|<span data-ttu-id="6d2fb-166">Binário Base64 de configuração do aplicativo MDM.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-166">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="6d2fb-167">configurações</span><span class="sxs-lookup"><span data-stu-id="6d2fb-167">settings</span></span>|<span data-ttu-id="6d2fb-168">Coleção de [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="6d2fb-168">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="6d2fb-169">Itens de configuração de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-169">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="6d2fb-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d2fb-170">Response</span></span>
<span data-ttu-id="6d2fb-171">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-171">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d2fb-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d2fb-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d2fb-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d2fb-173">Request</span></span>
<span data-ttu-id="6d2fb-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 596

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="6d2fb-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d2fb-175">Response</span></span>
<span data-ttu-id="6d2fb-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d2fb-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 768

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```





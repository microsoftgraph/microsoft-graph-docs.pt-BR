---
title: Atualizar iosMobileAppConfiguration
description: Atualiza as propriedades de um objeto iosMobileAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5a79cec9956670ad0be3f24118d8692ee06a5505
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39925778"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="0a133-103">Atualizar iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="0a133-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="0a133-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0a133-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a133-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a133-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a133-106">Atualiza as propriedades de um objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a133-106">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a133-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0a133-107">Prerequisites</span></span>
<span data-ttu-id="0a133-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a133-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a133-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a133-110">Permission type</span></span>|<span data-ttu-id="0a133-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0a133-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a133-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a133-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a133-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a133-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0a133-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a133-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a133-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a133-115">Not supported.</span></span>|
|<span data-ttu-id="0a133-116">Application</span><span class="sxs-lookup"><span data-stu-id="0a133-116">Application</span></span>|<span data-ttu-id="0a133-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a133-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a133-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a133-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0a133-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a133-119">Request headers</span></span>
|<span data-ttu-id="0a133-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a133-120">Header</span></span>|<span data-ttu-id="0a133-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0a133-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a133-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a133-122">Authorization</span></span>|<span data-ttu-id="0a133-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a133-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a133-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0a133-124">Accept</span></span>|<span data-ttu-id="0a133-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a133-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a133-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a133-126">Request body</span></span>
<span data-ttu-id="0a133-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a133-127">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="0a133-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a133-128">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="0a133-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a133-129">Property</span></span>|<span data-ttu-id="0a133-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a133-130">Type</span></span>|<span data-ttu-id="0a133-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a133-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a133-132">id</span><span class="sxs-lookup"><span data-stu-id="0a133-132">id</span></span>|<span data-ttu-id="0a133-133">String</span><span class="sxs-lookup"><span data-stu-id="0a133-133">String</span></span>|<span data-ttu-id="0a133-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0a133-134">Key of the entity.</span></span> <span data-ttu-id="0a133-135">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a133-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0a133-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="0a133-136">targetedMobileApps</span></span>|<span data-ttu-id="0a133-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a133-137">String collection</span></span>|<span data-ttu-id="0a133-138">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="0a133-138">the associated app.</span></span> <span data-ttu-id="0a133-139">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a133-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0a133-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0a133-140">roleScopeTagIds</span></span>|<span data-ttu-id="0a133-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a133-141">String collection</span></span>|<span data-ttu-id="0a133-142">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0a133-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="0a133-143">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a133-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0a133-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a133-144">createdDateTime</span></span>|<span data-ttu-id="0a133-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a133-145">DateTimeOffset</span></span>|<span data-ttu-id="0a133-146">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0a133-146">DateTime the object was created.</span></span> <span data-ttu-id="0a133-147">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a133-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0a133-148">description</span><span class="sxs-lookup"><span data-stu-id="0a133-148">description</span></span>|<span data-ttu-id="0a133-149">String</span><span class="sxs-lookup"><span data-stu-id="0a133-149">String</span></span>|<span data-ttu-id="0a133-150">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0a133-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0a133-151">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a133-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0a133-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a133-152">lastModifiedDateTime</span></span>|<span data-ttu-id="0a133-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a133-153">DateTimeOffset</span></span>|<span data-ttu-id="0a133-154">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0a133-154">DateTime the object was last modified.</span></span> <span data-ttu-id="0a133-155">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a133-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0a133-156">displayName</span><span class="sxs-lookup"><span data-stu-id="0a133-156">displayName</span></span>|<span data-ttu-id="0a133-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a133-157">String</span></span>|<span data-ttu-id="0a133-158">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0a133-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0a133-159">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a133-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0a133-160">version</span><span class="sxs-lookup"><span data-stu-id="0a133-160">version</span></span>|<span data-ttu-id="0a133-161">Int32</span><span class="sxs-lookup"><span data-stu-id="0a133-161">Int32</span></span>|<span data-ttu-id="0a133-162">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0a133-162">Version of the device configuration.</span></span> <span data-ttu-id="0a133-163">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a133-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0a133-164">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="0a133-164">encodedSettingXml</span></span>|<span data-ttu-id="0a133-165">Binária</span><span class="sxs-lookup"><span data-stu-id="0a133-165">Binary</span></span>|<span data-ttu-id="0a133-166">Binário Base64 de configuração do aplicativo MDM.</span><span class="sxs-lookup"><span data-stu-id="0a133-166">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="0a133-167">configurações</span><span class="sxs-lookup"><span data-stu-id="0a133-167">settings</span></span>|<span data-ttu-id="0a133-168">Coleção de [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="0a133-168">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="0a133-169">Itens de configuração de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0a133-169">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="0a133-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a133-170">Response</span></span>
<span data-ttu-id="0a133-171">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a133-171">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a133-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a133-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a133-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a133-173">Request</span></span>
<span data-ttu-id="0a133-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a133-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0a133-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a133-175">Response</span></span>
<span data-ttu-id="0a133-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a133-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






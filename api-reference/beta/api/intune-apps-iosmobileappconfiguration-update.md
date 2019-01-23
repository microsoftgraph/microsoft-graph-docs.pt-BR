---
title: Atualizar iosMobileAppConfiguration
description: Atualiza as propriedades de um objeto iosMobileAppConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aeb7ab2fc660b22c229342ddb78a7caa5e12dc70
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409899"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="99d8f-103">Atualizar iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="99d8f-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="99d8f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="99d8f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="99d8f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="99d8f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99d8f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="99d8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99d8f-107">Atualiza as propriedades de um objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99d8f-107">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99d8f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99d8f-108">Prerequisites</span></span>
<span data-ttu-id="99d8f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="99d8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="99d8f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99d8f-111">Permission type</span></span>|<span data-ttu-id="99d8f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="99d8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99d8f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99d8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99d8f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99d8f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="99d8f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99d8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99d8f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99d8f-116">Not supported.</span></span>|
|<span data-ttu-id="99d8f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99d8f-117">Application</span></span>|<span data-ttu-id="99d8f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99d8f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99d8f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99d8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="99d8f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99d8f-120">Request headers</span></span>
|<span data-ttu-id="99d8f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99d8f-121">Header</span></span>|<span data-ttu-id="99d8f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="99d8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99d8f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="99d8f-123">Authorization</span></span>|<span data-ttu-id="99d8f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99d8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99d8f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="99d8f-125">Accept</span></span>|<span data-ttu-id="99d8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99d8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99d8f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99d8f-127">Request body</span></span>
<span data-ttu-id="99d8f-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99d8f-128">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="99d8f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99d8f-129">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="99d8f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99d8f-130">Property</span></span>|<span data-ttu-id="99d8f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="99d8f-131">Type</span></span>|<span data-ttu-id="99d8f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="99d8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99d8f-133">id</span><span class="sxs-lookup"><span data-stu-id="99d8f-133">id</span></span>|<span data-ttu-id="99d8f-134">String</span><span class="sxs-lookup"><span data-stu-id="99d8f-134">String</span></span>|<span data-ttu-id="99d8f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="99d8f-135">Key of the entity.</span></span> <span data-ttu-id="99d8f-136">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99d8f-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="99d8f-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="99d8f-137">targetedMobileApps</span></span>|<span data-ttu-id="99d8f-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="99d8f-138">String collection</span></span>|<span data-ttu-id="99d8f-139">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="99d8f-139">the associated app.</span></span> <span data-ttu-id="99d8f-140">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99d8f-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="99d8f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="99d8f-141">roleScopeTagIds</span></span>|<span data-ttu-id="99d8f-142">String collection</span><span class="sxs-lookup"><span data-stu-id="99d8f-142">String collection</span></span>|<span data-ttu-id="99d8f-143">Lista de escopo marcas para essa entidade de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="99d8f-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="99d8f-144">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99d8f-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="99d8f-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99d8f-145">createdDateTime</span></span>|<span data-ttu-id="99d8f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99d8f-146">DateTimeOffset</span></span>|<span data-ttu-id="99d8f-147">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="99d8f-147">DateTime the object was created.</span></span> <span data-ttu-id="99d8f-148">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99d8f-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="99d8f-149">description</span><span class="sxs-lookup"><span data-stu-id="99d8f-149">description</span></span>|<span data-ttu-id="99d8f-150">String</span><span class="sxs-lookup"><span data-stu-id="99d8f-150">String</span></span>|<span data-ttu-id="99d8f-151">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="99d8f-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="99d8f-152">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99d8f-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="99d8f-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99d8f-153">lastModifiedDateTime</span></span>|<span data-ttu-id="99d8f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99d8f-154">DateTimeOffset</span></span>|<span data-ttu-id="99d8f-155">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="99d8f-155">DateTime the object was last modified.</span></span> <span data-ttu-id="99d8f-156">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99d8f-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="99d8f-157">displayName</span><span class="sxs-lookup"><span data-stu-id="99d8f-157">displayName</span></span>|<span data-ttu-id="99d8f-158">String</span><span class="sxs-lookup"><span data-stu-id="99d8f-158">String</span></span>|<span data-ttu-id="99d8f-159">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="99d8f-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="99d8f-160">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99d8f-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="99d8f-161">version</span><span class="sxs-lookup"><span data-stu-id="99d8f-161">version</span></span>|<span data-ttu-id="99d8f-162">Int32</span><span class="sxs-lookup"><span data-stu-id="99d8f-162">Int32</span></span>|<span data-ttu-id="99d8f-163">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="99d8f-163">Version of the device configuration.</span></span> <span data-ttu-id="99d8f-164">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99d8f-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="99d8f-165">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="99d8f-165">encodedSettingXml</span></span>|<span data-ttu-id="99d8f-166">Binária</span><span class="sxs-lookup"><span data-stu-id="99d8f-166">Binary</span></span>|<span data-ttu-id="99d8f-167">Binário Base64 de configuração do aplicativo MDM.</span><span class="sxs-lookup"><span data-stu-id="99d8f-167">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="99d8f-168">configurações</span><span class="sxs-lookup"><span data-stu-id="99d8f-168">settings</span></span>|<span data-ttu-id="99d8f-169">Coleção de [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="99d8f-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="99d8f-170">Itens de configuração de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="99d8f-170">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="99d8f-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="99d8f-171">Response</span></span>
<span data-ttu-id="99d8f-172">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99d8f-172">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99d8f-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99d8f-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="99d8f-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99d8f-174">Request</span></span>
<span data-ttu-id="99d8f-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99d8f-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="99d8f-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="99d8f-176">Response</span></span>
<span data-ttu-id="99d8f-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99d8f-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





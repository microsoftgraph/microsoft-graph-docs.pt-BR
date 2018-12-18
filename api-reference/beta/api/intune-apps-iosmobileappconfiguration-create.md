---
title: Criar iosMobileAppConfiguration
description: Cria um novo objeto iosMobileAppConfiguration.
author: tfitzmac
ms.openlocfilehash: e61a90540e0541fd9b14f4cad33e8ea9f95a803a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315782"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="46730-103">Criar iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="46730-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="46730-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="46730-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46730-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="46730-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46730-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="46730-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46730-107">Cria um novo objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46730-107">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46730-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="46730-108">Prerequisites</span></span>
<span data-ttu-id="46730-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46730-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46730-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46730-111">Permission type</span></span>|<span data-ttu-id="46730-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="46730-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46730-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46730-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46730-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46730-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="46730-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46730-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46730-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46730-116">Not supported.</span></span>|
|<span data-ttu-id="46730-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46730-117">Application</span></span>|<span data-ttu-id="46730-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46730-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46730-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46730-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="46730-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46730-120">Request headers</span></span>
|<span data-ttu-id="46730-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="46730-121">Header</span></span>|<span data-ttu-id="46730-122">Valor</span><span class="sxs-lookup"><span data-stu-id="46730-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46730-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="46730-123">Authorization</span></span>|<span data-ttu-id="46730-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46730-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46730-125">Accept</span><span class="sxs-lookup"><span data-stu-id="46730-125">Accept</span></span>|<span data-ttu-id="46730-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46730-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46730-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46730-127">Request body</span></span>
<span data-ttu-id="46730-128">No corpo da solicitação, forneça uma representação JSON do objeto iosMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="46730-128">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="46730-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o iosMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="46730-129">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="46730-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46730-130">Property</span></span>|<span data-ttu-id="46730-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="46730-131">Type</span></span>|<span data-ttu-id="46730-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="46730-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46730-133">id</span><span class="sxs-lookup"><span data-stu-id="46730-133">id</span></span>|<span data-ttu-id="46730-134">String</span><span class="sxs-lookup"><span data-stu-id="46730-134">String</span></span>|<span data-ttu-id="46730-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="46730-135">Key of the entity.</span></span> <span data-ttu-id="46730-136">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46730-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="46730-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="46730-137">targetedMobileApps</span></span>|<span data-ttu-id="46730-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="46730-138">String collection</span></span>|<span data-ttu-id="46730-139">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="46730-139">the associated app.</span></span> <span data-ttu-id="46730-140">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46730-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="46730-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="46730-141">roleScopeTagIds</span></span>|<span data-ttu-id="46730-142">String collection</span><span class="sxs-lookup"><span data-stu-id="46730-142">String collection</span></span>|<span data-ttu-id="46730-143">Lista de escopo marcas para essa entidade de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="46730-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="46730-144">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46730-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="46730-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="46730-145">createdDateTime</span></span>|<span data-ttu-id="46730-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46730-146">DateTimeOffset</span></span>|<span data-ttu-id="46730-147">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="46730-147">DateTime the object was created.</span></span> <span data-ttu-id="46730-148">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46730-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="46730-149">description</span><span class="sxs-lookup"><span data-stu-id="46730-149">description</span></span>|<span data-ttu-id="46730-150">String</span><span class="sxs-lookup"><span data-stu-id="46730-150">String</span></span>|<span data-ttu-id="46730-151">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="46730-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="46730-152">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46730-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="46730-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="46730-153">lastModifiedDateTime</span></span>|<span data-ttu-id="46730-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46730-154">DateTimeOffset</span></span>|<span data-ttu-id="46730-155">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="46730-155">DateTime the object was last modified.</span></span> <span data-ttu-id="46730-156">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46730-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="46730-157">displayName</span><span class="sxs-lookup"><span data-stu-id="46730-157">displayName</span></span>|<span data-ttu-id="46730-158">String</span><span class="sxs-lookup"><span data-stu-id="46730-158">String</span></span>|<span data-ttu-id="46730-159">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="46730-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="46730-160">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46730-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="46730-161">version</span><span class="sxs-lookup"><span data-stu-id="46730-161">version</span></span>|<span data-ttu-id="46730-162">Int32</span><span class="sxs-lookup"><span data-stu-id="46730-162">Int32</span></span>|<span data-ttu-id="46730-163">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="46730-163">Version of the device configuration.</span></span> <span data-ttu-id="46730-164">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46730-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="46730-165">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="46730-165">encodedSettingXml</span></span>|<span data-ttu-id="46730-166">Binária</span><span class="sxs-lookup"><span data-stu-id="46730-166">Binary</span></span>|<span data-ttu-id="46730-167">Binário Base64 de configuração do aplicativo MDM.</span><span class="sxs-lookup"><span data-stu-id="46730-167">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="46730-168">configurações</span><span class="sxs-lookup"><span data-stu-id="46730-168">settings</span></span>|<span data-ttu-id="46730-169">Coleção de [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="46730-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="46730-170">Itens de configuração de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="46730-170">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="46730-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="46730-171">Response</span></span>
<span data-ttu-id="46730-172">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46730-172">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46730-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46730-173">Example</span></span>
### <a name="request"></a><span data-ttu-id="46730-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46730-174">Request</span></span>
<span data-ttu-id="46730-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46730-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 660

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="46730-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="46730-176">Response</span></span>
<span data-ttu-id="46730-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46730-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






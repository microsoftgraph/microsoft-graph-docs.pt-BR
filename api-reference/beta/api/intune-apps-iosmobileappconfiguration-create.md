---
title: Criar iosMobileAppConfiguration
description: Cria um novo objeto iosMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3e9668794b582479fdc4ab0cee50519a1c1e12ca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939942"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="cfe5a-103">Criar iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cfe5a-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="cfe5a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cfe5a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cfe5a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cfe5a-107">Cria um novo objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfe5a-107">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cfe5a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cfe5a-108">Prerequisites</span></span>
<span data-ttu-id="cfe5a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfe5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfe5a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfe5a-111">Permission type</span></span>|<span data-ttu-id="cfe5a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cfe5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfe5a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfe5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cfe5a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfe5a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cfe5a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfe5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfe5a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-116">Not supported.</span></span>|
|<span data-ttu-id="cfe5a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cfe5a-117">Application</span></span>|<span data-ttu-id="cfe5a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfe5a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfe5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cfe5a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfe5a-120">Request headers</span></span>
|<span data-ttu-id="cfe5a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cfe5a-121">Header</span></span>|<span data-ttu-id="cfe5a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cfe5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfe5a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfe5a-123">Authorization</span></span>|<span data-ttu-id="cfe5a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfe5a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cfe5a-125">Accept</span></span>|<span data-ttu-id="cfe5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cfe5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfe5a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfe5a-127">Request body</span></span>
<span data-ttu-id="cfe5a-128">No corpo da solicitação, forneça uma representação JSON do objeto iosMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-128">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="cfe5a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o iosMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-129">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="cfe5a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfe5a-130">Property</span></span>|<span data-ttu-id="cfe5a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfe5a-131">Type</span></span>|<span data-ttu-id="cfe5a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfe5a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfe5a-133">id</span><span class="sxs-lookup"><span data-stu-id="cfe5a-133">id</span></span>|<span data-ttu-id="cfe5a-134">String</span><span class="sxs-lookup"><span data-stu-id="cfe5a-134">String</span></span>|<span data-ttu-id="cfe5a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-135">Key of the entity.</span></span> <span data-ttu-id="cfe5a-136">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cfe5a-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cfe5a-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="cfe5a-137">targetedMobileApps</span></span>|<span data-ttu-id="cfe5a-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfe5a-138">String collection</span></span>|<span data-ttu-id="cfe5a-139">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-139">the associated app.</span></span> <span data-ttu-id="cfe5a-140">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cfe5a-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cfe5a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cfe5a-141">roleScopeTagIds</span></span>|<span data-ttu-id="cfe5a-142">String collection</span><span class="sxs-lookup"><span data-stu-id="cfe5a-142">String collection</span></span>|<span data-ttu-id="cfe5a-143">Lista de escopo marcas para essa entidade de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="cfe5a-144">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cfe5a-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cfe5a-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cfe5a-145">createdDateTime</span></span>|<span data-ttu-id="cfe5a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfe5a-146">DateTimeOffset</span></span>|<span data-ttu-id="cfe5a-147">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-147">DateTime the object was created.</span></span> <span data-ttu-id="cfe5a-148">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cfe5a-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cfe5a-149">description</span><span class="sxs-lookup"><span data-stu-id="cfe5a-149">description</span></span>|<span data-ttu-id="cfe5a-150">String</span><span class="sxs-lookup"><span data-stu-id="cfe5a-150">String</span></span>|<span data-ttu-id="cfe5a-151">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cfe5a-152">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cfe5a-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cfe5a-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cfe5a-153">lastModifiedDateTime</span></span>|<span data-ttu-id="cfe5a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfe5a-154">DateTimeOffset</span></span>|<span data-ttu-id="cfe5a-155">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-155">DateTime the object was last modified.</span></span> <span data-ttu-id="cfe5a-156">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cfe5a-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cfe5a-157">displayName</span><span class="sxs-lookup"><span data-stu-id="cfe5a-157">displayName</span></span>|<span data-ttu-id="cfe5a-158">String</span><span class="sxs-lookup"><span data-stu-id="cfe5a-158">String</span></span>|<span data-ttu-id="cfe5a-159">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cfe5a-160">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cfe5a-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cfe5a-161">version</span><span class="sxs-lookup"><span data-stu-id="cfe5a-161">version</span></span>|<span data-ttu-id="cfe5a-162">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe5a-162">Int32</span></span>|<span data-ttu-id="cfe5a-163">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-163">Version of the device configuration.</span></span> <span data-ttu-id="cfe5a-164">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cfe5a-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cfe5a-165">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="cfe5a-165">encodedSettingXml</span></span>|<span data-ttu-id="cfe5a-166">Binária</span><span class="sxs-lookup"><span data-stu-id="cfe5a-166">Binary</span></span>|<span data-ttu-id="cfe5a-167">Binário Base64 de configuração do aplicativo MDM.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-167">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="cfe5a-168">configurações</span><span class="sxs-lookup"><span data-stu-id="cfe5a-168">settings</span></span>|<span data-ttu-id="cfe5a-169">Coleção de [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="cfe5a-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="cfe5a-170">Itens de configuração de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-170">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="cfe5a-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfe5a-171">Response</span></span>
<span data-ttu-id="cfe5a-172">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-172">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfe5a-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cfe5a-173">Example</span></span>
### <a name="request"></a><span data-ttu-id="cfe5a-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfe5a-174">Request</span></span>
<span data-ttu-id="cfe5a-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cfe5a-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfe5a-176">Response</span></span>
<span data-ttu-id="cfe5a-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfe5a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






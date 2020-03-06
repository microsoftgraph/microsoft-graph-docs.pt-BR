---
title: Criar iosMobileAppConfiguration
description: Cria um novo objeto iosMobileAppConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c981cd33dbb125e41bd2a151d5dbc5e2d189d847
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516585"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="cd41f-103">Criar iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd41f-103">Create iosMobileAppConfiguration</span></span>

<span data-ttu-id="cd41f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd41f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd41f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cd41f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd41f-106">Cria um novo objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cd41f-106">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd41f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cd41f-107">Prerequisites</span></span>
<span data-ttu-id="cd41f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd41f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd41f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd41f-110">Permission type</span></span>|<span data-ttu-id="cd41f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cd41f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd41f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd41f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd41f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd41f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cd41f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd41f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd41f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd41f-115">Not supported.</span></span>|
|<span data-ttu-id="cd41f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd41f-116">Application</span></span>|<span data-ttu-id="cd41f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd41f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd41f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd41f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cd41f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd41f-119">Request headers</span></span>
|<span data-ttu-id="cd41f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cd41f-120">Header</span></span>|<span data-ttu-id="cd41f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cd41f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd41f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd41f-122">Authorization</span></span>|<span data-ttu-id="cd41f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd41f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd41f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cd41f-124">Accept</span></span>|<span data-ttu-id="cd41f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd41f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd41f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd41f-126">Request body</span></span>
<span data-ttu-id="cd41f-127">No corpo da solicitação, forneça uma representação JSON do objeto iosMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cd41f-127">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="cd41f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar o iosMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cd41f-128">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="cd41f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd41f-129">Property</span></span>|<span data-ttu-id="cd41f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd41f-130">Type</span></span>|<span data-ttu-id="cd41f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd41f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd41f-132">id</span><span class="sxs-lookup"><span data-stu-id="cd41f-132">id</span></span>|<span data-ttu-id="cd41f-133">String</span><span class="sxs-lookup"><span data-stu-id="cd41f-133">String</span></span>|<span data-ttu-id="cd41f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cd41f-134">Key of the entity.</span></span> <span data-ttu-id="cd41f-135">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd41f-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cd41f-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="cd41f-136">targetedMobileApps</span></span>|<span data-ttu-id="cd41f-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd41f-137">String collection</span></span>|<span data-ttu-id="cd41f-138">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="cd41f-138">the associated app.</span></span> <span data-ttu-id="cd41f-139">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd41f-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cd41f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd41f-140">createdDateTime</span></span>|<span data-ttu-id="cd41f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd41f-141">DateTimeOffset</span></span>|<span data-ttu-id="cd41f-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="cd41f-142">DateTime the object was created.</span></span> <span data-ttu-id="cd41f-143">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd41f-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cd41f-144">description</span><span class="sxs-lookup"><span data-stu-id="cd41f-144">description</span></span>|<span data-ttu-id="cd41f-145">String</span><span class="sxs-lookup"><span data-stu-id="cd41f-145">String</span></span>|<span data-ttu-id="cd41f-146">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cd41f-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cd41f-147">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd41f-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cd41f-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd41f-148">lastModifiedDateTime</span></span>|<span data-ttu-id="cd41f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd41f-149">DateTimeOffset</span></span>|<span data-ttu-id="cd41f-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="cd41f-150">DateTime the object was last modified.</span></span> <span data-ttu-id="cd41f-151">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd41f-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cd41f-152">displayName</span><span class="sxs-lookup"><span data-stu-id="cd41f-152">displayName</span></span>|<span data-ttu-id="cd41f-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd41f-153">String</span></span>|<span data-ttu-id="cd41f-154">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cd41f-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cd41f-155">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd41f-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cd41f-156">version</span><span class="sxs-lookup"><span data-stu-id="cd41f-156">version</span></span>|<span data-ttu-id="cd41f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="cd41f-157">Int32</span></span>|<span data-ttu-id="cd41f-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cd41f-158">Version of the device configuration.</span></span> <span data-ttu-id="cd41f-159">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd41f-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cd41f-160">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="cd41f-160">encodedSettingXml</span></span>|<span data-ttu-id="cd41f-161">Binária</span><span class="sxs-lookup"><span data-stu-id="cd41f-161">Binary</span></span>|<span data-ttu-id="cd41f-162">Binário Base64 de configuração do aplicativo MDM.</span><span class="sxs-lookup"><span data-stu-id="cd41f-162">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="cd41f-163">configurações</span><span class="sxs-lookup"><span data-stu-id="cd41f-163">settings</span></span>|<span data-ttu-id="cd41f-164">Coleção de [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="cd41f-164">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="cd41f-165">Itens de configuração de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cd41f-165">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="cd41f-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd41f-166">Response</span></span>
<span data-ttu-id="cd41f-167">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd41f-167">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd41f-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd41f-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd41f-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd41f-169">Request</span></span>
<span data-ttu-id="cd41f-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd41f-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 534

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
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

### <a name="response"></a><span data-ttu-id="cd41f-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd41f-171">Response</span></span>
<span data-ttu-id="cd41f-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cd41f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 706

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
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





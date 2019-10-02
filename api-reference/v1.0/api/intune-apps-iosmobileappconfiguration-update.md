---
title: Atualizar iosMobileAppConfiguration
description: Atualiza as propriedades de um objeto iosMobileAppConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9f8a243745c821b15bf4108d15b47f055a160400
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358876"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="d93be-103">Atualizar iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d93be-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="d93be-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d93be-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d93be-105">Atualiza as propriedades de um objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d93be-105">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d93be-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d93be-106">Prerequisites</span></span>
<span data-ttu-id="d93be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d93be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d93be-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d93be-109">Permission type</span></span>|<span data-ttu-id="d93be-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d93be-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d93be-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d93be-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d93be-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d93be-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d93be-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d93be-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d93be-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d93be-114">Not supported.</span></span>|
|<span data-ttu-id="d93be-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d93be-115">Application</span></span>|<span data-ttu-id="d93be-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d93be-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d93be-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d93be-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d93be-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d93be-118">Request headers</span></span>
|<span data-ttu-id="d93be-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d93be-119">Header</span></span>|<span data-ttu-id="d93be-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d93be-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d93be-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d93be-121">Authorization</span></span>|<span data-ttu-id="d93be-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d93be-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d93be-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d93be-123">Accept</span></span>|<span data-ttu-id="d93be-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d93be-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d93be-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d93be-125">Request body</span></span>
<span data-ttu-id="d93be-126">No corpo da solicitação, forneça uma representação JSON do objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d93be-126">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="d93be-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d93be-127">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="d93be-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d93be-128">Property</span></span>|<span data-ttu-id="d93be-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d93be-129">Type</span></span>|<span data-ttu-id="d93be-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d93be-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d93be-131">id</span><span class="sxs-lookup"><span data-stu-id="d93be-131">id</span></span>|<span data-ttu-id="d93be-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d93be-132">String</span></span>|<span data-ttu-id="d93be-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d93be-133">Key of the entity.</span></span> <span data-ttu-id="d93be-134">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d93be-134">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d93be-135">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="d93be-135">targetedMobileApps</span></span>|<span data-ttu-id="d93be-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d93be-136">String collection</span></span>|<span data-ttu-id="d93be-137">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="d93be-137">the associated app.</span></span> <span data-ttu-id="d93be-138">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d93be-138">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d93be-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d93be-139">createdDateTime</span></span>|<span data-ttu-id="d93be-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d93be-140">DateTimeOffset</span></span>|<span data-ttu-id="d93be-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d93be-141">DateTime the object was created.</span></span> <span data-ttu-id="d93be-142">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d93be-142">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d93be-143">descrição</span><span class="sxs-lookup"><span data-stu-id="d93be-143">description</span></span>|<span data-ttu-id="d93be-144">String</span><span class="sxs-lookup"><span data-stu-id="d93be-144">String</span></span>|<span data-ttu-id="d93be-145">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d93be-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d93be-146">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d93be-146">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d93be-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d93be-147">lastModifiedDateTime</span></span>|<span data-ttu-id="d93be-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d93be-148">DateTimeOffset</span></span>|<span data-ttu-id="d93be-149">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d93be-149">DateTime the object was last modified.</span></span> <span data-ttu-id="d93be-150">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d93be-150">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d93be-151">displayName</span><span class="sxs-lookup"><span data-stu-id="d93be-151">displayName</span></span>|<span data-ttu-id="d93be-152">String</span><span class="sxs-lookup"><span data-stu-id="d93be-152">String</span></span>|<span data-ttu-id="d93be-153">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d93be-153">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d93be-154">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d93be-154">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d93be-155">version</span><span class="sxs-lookup"><span data-stu-id="d93be-155">version</span></span>|<span data-ttu-id="d93be-156">Int32</span><span class="sxs-lookup"><span data-stu-id="d93be-156">Int32</span></span>|<span data-ttu-id="d93be-157">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d93be-157">Version of the device configuration.</span></span> <span data-ttu-id="d93be-158">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d93be-158">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d93be-159">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="d93be-159">encodedSettingXml</span></span>|<span data-ttu-id="d93be-160">Binária</span><span class="sxs-lookup"><span data-stu-id="d93be-160">Binary</span></span>|<span data-ttu-id="d93be-161">Binário Base64 de configuração do aplicativo MDM.</span><span class="sxs-lookup"><span data-stu-id="d93be-161">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="d93be-162">configurações</span><span class="sxs-lookup"><span data-stu-id="d93be-162">settings</span></span>|<span data-ttu-id="d93be-163">Coleção de [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="d93be-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="d93be-164">Itens de configuração de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d93be-164">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="d93be-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="d93be-165">Response</span></span>
<span data-ttu-id="d93be-166">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d93be-166">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d93be-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d93be-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="d93be-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d93be-168">Request</span></span>
<span data-ttu-id="d93be-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d93be-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
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

### <a name="response"></a><span data-ttu-id="d93be-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="d93be-170">Response</span></span>
<span data-ttu-id="d93be-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d93be-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





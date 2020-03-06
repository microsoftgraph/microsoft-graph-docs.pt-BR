---
title: Atualizar iosDeviceFeaturesConfiguration
description: Atualizar as propriedades de um objeto iosDeviceFeaturesConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4bd08c4c4dbfa0e74f4c634f067dc428a41b7fb6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514540"
---
# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="13bd0-103">Atualizar iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="13bd0-103">Update iosDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="13bd0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13bd0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13bd0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13bd0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13bd0-106">Atualizar as propriedades de um objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13bd0-106">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13bd0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13bd0-107">Prerequisites</span></span>
<span data-ttu-id="13bd0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13bd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13bd0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13bd0-110">Permission type</span></span>|<span data-ttu-id="13bd0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13bd0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13bd0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13bd0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13bd0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13bd0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13bd0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13bd0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13bd0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13bd0-115">Not supported.</span></span>|
|<span data-ttu-id="13bd0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13bd0-116">Application</span></span>|<span data-ttu-id="13bd0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13bd0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13bd0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13bd0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="13bd0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13bd0-119">Request headers</span></span>
|<span data-ttu-id="13bd0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13bd0-120">Header</span></span>|<span data-ttu-id="13bd0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="13bd0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13bd0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="13bd0-122">Authorization</span></span>|<span data-ttu-id="13bd0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13bd0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13bd0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13bd0-124">Accept</span></span>|<span data-ttu-id="13bd0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13bd0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13bd0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13bd0-126">Request body</span></span>
<span data-ttu-id="13bd0-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13bd0-127">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="13bd0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13bd0-128">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="13bd0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13bd0-129">Property</span></span>|<span data-ttu-id="13bd0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="13bd0-130">Type</span></span>|<span data-ttu-id="13bd0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="13bd0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13bd0-132">id</span><span class="sxs-lookup"><span data-stu-id="13bd0-132">id</span></span>|<span data-ttu-id="13bd0-133">String</span><span class="sxs-lookup"><span data-stu-id="13bd0-133">String</span></span>|<span data-ttu-id="13bd0-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="13bd0-134">Key of the entity.</span></span> <span data-ttu-id="13bd0-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13bd0-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13bd0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13bd0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="13bd0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13bd0-137">DateTimeOffset</span></span>|<span data-ttu-id="13bd0-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="13bd0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="13bd0-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13bd0-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13bd0-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13bd0-140">createdDateTime</span></span>|<span data-ttu-id="13bd0-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13bd0-141">DateTimeOffset</span></span>|<span data-ttu-id="13bd0-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="13bd0-142">DateTime the object was created.</span></span> <span data-ttu-id="13bd0-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13bd0-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13bd0-144">description</span><span class="sxs-lookup"><span data-stu-id="13bd0-144">description</span></span>|<span data-ttu-id="13bd0-145">String</span><span class="sxs-lookup"><span data-stu-id="13bd0-145">String</span></span>|<span data-ttu-id="13bd0-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13bd0-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="13bd0-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13bd0-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13bd0-148">displayName</span><span class="sxs-lookup"><span data-stu-id="13bd0-148">displayName</span></span>|<span data-ttu-id="13bd0-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13bd0-149">String</span></span>|<span data-ttu-id="13bd0-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13bd0-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="13bd0-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13bd0-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13bd0-152">versão</span><span class="sxs-lookup"><span data-stu-id="13bd0-152">version</span></span>|<span data-ttu-id="13bd0-153">Int32</span><span class="sxs-lookup"><span data-stu-id="13bd0-153">Int32</span></span>|<span data-ttu-id="13bd0-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13bd0-154">Version of the device configuration.</span></span> <span data-ttu-id="13bd0-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13bd0-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13bd0-156">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="13bd0-156">assetTagTemplate</span></span>|<span data-ttu-id="13bd0-157">String</span><span class="sxs-lookup"><span data-stu-id="13bd0-157">String</span></span>|<span data-ttu-id="13bd0-158">Informações de marcação de ativos para o dispositivo, exibidas na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="13bd0-158">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="13bd0-159">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="13bd0-159">lockScreenFootnote</span></span>|<span data-ttu-id="13bd0-160">String</span><span class="sxs-lookup"><span data-stu-id="13bd0-160">String</span></span>|<span data-ttu-id="13bd0-161">Uma nota de rodapé exibida na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="13bd0-161">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="13bd0-162">Disponível no iOS 9.3.1 e posterior.</span><span class="sxs-lookup"><span data-stu-id="13bd0-162">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="13bd0-163">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="13bd0-163">homeScreenDockIcons</span></span>|<span data-ttu-id="13bd0-164">Coleção [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="13bd0-164">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="13bd0-165">Uma lista dos aplicativos e pastas exibidos em um dock de tela inicial.</span><span class="sxs-lookup"><span data-stu-id="13bd0-165">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="13bd0-166">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="13bd0-166">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="13bd0-167">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="13bd0-167">homeScreenPages</span></span>|<span data-ttu-id="13bd0-168">Coleção [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="13bd0-168">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="13bd0-169">Uma lista de páginas na tela inicial.</span><span class="sxs-lookup"><span data-stu-id="13bd0-169">A list of pages on the Home Screen.</span></span> <span data-ttu-id="13bd0-170">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="13bd0-170">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="13bd0-171">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="13bd0-171">notificationSettings</span></span>|<span data-ttu-id="13bd0-172">Coleção [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="13bd0-172">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="13bd0-173">Configurações de notificação para cada ID de pacote. Aplicáveis apenas a dispositivos no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="13bd0-173">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="13bd0-174">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="13bd0-174">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="13bd0-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="13bd0-175">Response</span></span>
<span data-ttu-id="13bd0-176">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13bd0-176">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13bd0-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13bd0-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="13bd0-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13bd0-178">Request</span></span>
<span data-ttu-id="13bd0-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13bd0-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="13bd0-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="13bd0-180">Response</span></span>
<span data-ttu-id="13bd0-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13bd0-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2160

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```





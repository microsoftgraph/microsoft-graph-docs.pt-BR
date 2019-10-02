---
title: Atualizar iosDeviceFeaturesConfiguration
description: Atualizar as propriedades de um objeto iosDeviceFeaturesConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 562a7c1f3d509780b5750a2061963b2304fd6094
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366346"
---
# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="8ff91-103">Atualizar iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ff91-103">Update iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="8ff91-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ff91-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ff91-105">Atualizar as propriedades de um objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ff91-105">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ff91-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8ff91-106">Prerequisites</span></span>
<span data-ttu-id="8ff91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ff91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ff91-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ff91-109">Permission type</span></span>|<span data-ttu-id="8ff91-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8ff91-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ff91-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ff91-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8ff91-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ff91-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ff91-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ff91-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ff91-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ff91-114">Not supported.</span></span>|
|<span data-ttu-id="8ff91-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ff91-115">Application</span></span>|<span data-ttu-id="8ff91-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ff91-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ff91-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ff91-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8ff91-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff91-118">Request headers</span></span>
|<span data-ttu-id="8ff91-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ff91-119">Header</span></span>|<span data-ttu-id="8ff91-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8ff91-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ff91-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ff91-121">Authorization</span></span>|<span data-ttu-id="8ff91-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ff91-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ff91-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8ff91-123">Accept</span></span>|<span data-ttu-id="8ff91-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8ff91-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ff91-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff91-125">Request body</span></span>
<span data-ttu-id="8ff91-126">No corpo da solicitação, forneça uma representação JSON do objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ff91-126">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="8ff91-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ff91-127">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="8ff91-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ff91-128">Property</span></span>|<span data-ttu-id="8ff91-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ff91-129">Type</span></span>|<span data-ttu-id="8ff91-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ff91-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ff91-131">id</span><span class="sxs-lookup"><span data-stu-id="8ff91-131">id</span></span>|<span data-ttu-id="8ff91-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ff91-132">String</span></span>|<span data-ttu-id="8ff91-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8ff91-133">Key of the entity.</span></span> <span data-ttu-id="8ff91-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ff91-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff91-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ff91-135">lastModifiedDateTime</span></span>|<span data-ttu-id="8ff91-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ff91-136">DateTimeOffset</span></span>|<span data-ttu-id="8ff91-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8ff91-137">DateTime the object was last modified.</span></span> <span data-ttu-id="8ff91-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ff91-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff91-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ff91-139">createdDateTime</span></span>|<span data-ttu-id="8ff91-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ff91-140">DateTimeOffset</span></span>|<span data-ttu-id="8ff91-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8ff91-141">DateTime the object was created.</span></span> <span data-ttu-id="8ff91-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ff91-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff91-143">descrição</span><span class="sxs-lookup"><span data-stu-id="8ff91-143">description</span></span>|<span data-ttu-id="8ff91-144">String</span><span class="sxs-lookup"><span data-stu-id="8ff91-144">String</span></span>|<span data-ttu-id="8ff91-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8ff91-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8ff91-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ff91-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff91-147">displayName</span><span class="sxs-lookup"><span data-stu-id="8ff91-147">displayName</span></span>|<span data-ttu-id="8ff91-148">String</span><span class="sxs-lookup"><span data-stu-id="8ff91-148">String</span></span>|<span data-ttu-id="8ff91-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8ff91-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8ff91-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ff91-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff91-151">versão</span><span class="sxs-lookup"><span data-stu-id="8ff91-151">version</span></span>|<span data-ttu-id="8ff91-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8ff91-152">Int32</span></span>|<span data-ttu-id="8ff91-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8ff91-153">Version of the device configuration.</span></span> <span data-ttu-id="8ff91-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ff91-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff91-155">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="8ff91-155">assetTagTemplate</span></span>|<span data-ttu-id="8ff91-156">String</span><span class="sxs-lookup"><span data-stu-id="8ff91-156">String</span></span>|<span data-ttu-id="8ff91-157">Informações de marcação de ativos para o dispositivo, exibidas na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="8ff91-157">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="8ff91-158">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="8ff91-158">lockScreenFootnote</span></span>|<span data-ttu-id="8ff91-159">String</span><span class="sxs-lookup"><span data-stu-id="8ff91-159">String</span></span>|<span data-ttu-id="8ff91-160">Uma nota de rodapé exibida na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="8ff91-160">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="8ff91-161">Disponível no iOS 9.3.1 e posterior.</span><span class="sxs-lookup"><span data-stu-id="8ff91-161">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="8ff91-162">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="8ff91-162">homeScreenDockIcons</span></span>|<span data-ttu-id="8ff91-163">Coleção [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="8ff91-163">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="8ff91-164">Uma lista dos aplicativos e pastas exibidos em um dock de tela inicial.</span><span class="sxs-lookup"><span data-stu-id="8ff91-164">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="8ff91-165">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="8ff91-165">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8ff91-166">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="8ff91-166">homeScreenPages</span></span>|<span data-ttu-id="8ff91-167">Coleção [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="8ff91-167">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="8ff91-168">Uma lista de páginas na tela inicial.</span><span class="sxs-lookup"><span data-stu-id="8ff91-168">A list of pages on the Home Screen.</span></span> <span data-ttu-id="8ff91-169">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="8ff91-169">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8ff91-170">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="8ff91-170">notificationSettings</span></span>|<span data-ttu-id="8ff91-171">Coleção [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8ff91-171">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="8ff91-172">Configurações de notificação para cada ID de pacote. Aplicáveis apenas a dispositivos no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="8ff91-172">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="8ff91-173">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="8ff91-173">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="8ff91-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ff91-174">Response</span></span>
<span data-ttu-id="8ff91-175">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ff91-175">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ff91-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ff91-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ff91-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff91-177">Request</span></span>
<span data-ttu-id="8ff91-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ff91-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8ff91-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ff91-179">Response</span></span>
<span data-ttu-id="8ff91-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ff91-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





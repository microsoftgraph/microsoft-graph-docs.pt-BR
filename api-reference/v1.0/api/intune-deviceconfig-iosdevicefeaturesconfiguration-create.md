---
title: Criar iosDeviceFeaturesConfiguration
description: Criar um novo objeto iosDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 159247c7bde00b98fd9f25275bcab1be74f034fb
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264257"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="419f9-103">Criar iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="419f9-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="419f9-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="419f9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="419f9-105">Criar um novo objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="419f9-105">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="419f9-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="419f9-106">Prerequisites</span></span>
<span data-ttu-id="419f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="419f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="419f9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="419f9-109">Permission type</span></span>|<span data-ttu-id="419f9-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="419f9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="419f9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="419f9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="419f9-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="419f9-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="419f9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="419f9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="419f9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="419f9-114">Not supported.</span></span>|
|<span data-ttu-id="419f9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="419f9-115">Application</span></span>|<span data-ttu-id="419f9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="419f9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="419f9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="419f9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="419f9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="419f9-118">Request headers</span></span>
|<span data-ttu-id="419f9-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="419f9-119">Header</span></span>|<span data-ttu-id="419f9-120">Valor</span><span class="sxs-lookup"><span data-stu-id="419f9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="419f9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="419f9-121">Authorization</span></span>|<span data-ttu-id="419f9-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="419f9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="419f9-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="419f9-123">Accept</span></span>|<span data-ttu-id="419f9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="419f9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="419f9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="419f9-125">Request body</span></span>
<span data-ttu-id="419f9-126">No corpo da solicitação, forneça uma representação JSON do objeto iosDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="419f9-126">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="419f9-127">A tabela a seguir mostra as propriedades que são necessárias ao criar iosDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="419f9-127">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="419f9-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="419f9-128">Property</span></span>|<span data-ttu-id="419f9-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="419f9-129">Type</span></span>|<span data-ttu-id="419f9-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="419f9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="419f9-131">id</span><span class="sxs-lookup"><span data-stu-id="419f9-131">id</span></span>|<span data-ttu-id="419f9-132">String</span><span class="sxs-lookup"><span data-stu-id="419f9-132">String</span></span>|<span data-ttu-id="419f9-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="419f9-133">Key of the entity.</span></span> <span data-ttu-id="419f9-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="419f9-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="419f9-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="419f9-135">lastModifiedDateTime</span></span>|<span data-ttu-id="419f9-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="419f9-136">DateTimeOffset</span></span>|<span data-ttu-id="419f9-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="419f9-137">DateTime the object was last modified.</span></span> <span data-ttu-id="419f9-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="419f9-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="419f9-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="419f9-139">createdDateTime</span></span>|<span data-ttu-id="419f9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="419f9-140">DateTimeOffset</span></span>|<span data-ttu-id="419f9-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="419f9-141">DateTime the object was created.</span></span> <span data-ttu-id="419f9-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="419f9-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="419f9-143">description</span><span class="sxs-lookup"><span data-stu-id="419f9-143">description</span></span>|<span data-ttu-id="419f9-144">String</span><span class="sxs-lookup"><span data-stu-id="419f9-144">String</span></span>|<span data-ttu-id="419f9-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="419f9-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="419f9-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="419f9-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="419f9-147">displayName</span><span class="sxs-lookup"><span data-stu-id="419f9-147">displayName</span></span>|<span data-ttu-id="419f9-148">String</span><span class="sxs-lookup"><span data-stu-id="419f9-148">String</span></span>|<span data-ttu-id="419f9-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="419f9-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="419f9-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="419f9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="419f9-151">version</span><span class="sxs-lookup"><span data-stu-id="419f9-151">version</span></span>|<span data-ttu-id="419f9-152">Int32</span><span class="sxs-lookup"><span data-stu-id="419f9-152">Int32</span></span>|<span data-ttu-id="419f9-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="419f9-153">Version of the device configuration.</span></span> <span data-ttu-id="419f9-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="419f9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="419f9-155">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="419f9-155">assetTagTemplate</span></span>|<span data-ttu-id="419f9-156">String</span><span class="sxs-lookup"><span data-stu-id="419f9-156">String</span></span>|<span data-ttu-id="419f9-157">Informações de marcação de ativos para o dispositivo, exibidas na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="419f9-157">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="419f9-158">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="419f9-158">lockScreenFootnote</span></span>|<span data-ttu-id="419f9-159">String</span><span class="sxs-lookup"><span data-stu-id="419f9-159">String</span></span>|<span data-ttu-id="419f9-160">Uma nota de rodapé exibida na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="419f9-160">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="419f9-161">Disponível no iOS 9.3.1 e posterior.</span><span class="sxs-lookup"><span data-stu-id="419f9-161">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="419f9-162">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="419f9-162">homeScreenDockIcons</span></span>|<span data-ttu-id="419f9-163">Coleção [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="419f9-163">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="419f9-164">Uma lista dos aplicativos e pastas exibidos em um dock de tela inicial.</span><span class="sxs-lookup"><span data-stu-id="419f9-164">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="419f9-165">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="419f9-165">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="419f9-166">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="419f9-166">homeScreenPages</span></span>|<span data-ttu-id="419f9-167">Coleção [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="419f9-167">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="419f9-168">Uma lista de páginas na tela inicial.</span><span class="sxs-lookup"><span data-stu-id="419f9-168">A list of pages on the Home Screen.</span></span> <span data-ttu-id="419f9-169">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="419f9-169">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="419f9-170">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="419f9-170">notificationSettings</span></span>|<span data-ttu-id="419f9-171">Coleção [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="419f9-171">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="419f9-172">Configurações de notificação para cada ID de pacote. Aplicáveis apenas a dispositivos no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="419f9-172">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="419f9-173">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="419f9-173">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="419f9-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="419f9-174">Response</span></span>
<span data-ttu-id="419f9-175">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="419f9-175">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="419f9-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="419f9-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="419f9-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="419f9-177">Request</span></span>
<span data-ttu-id="419f9-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="419f9-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="419f9-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="419f9-179">Response</span></span>
<span data-ttu-id="419f9-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="419f9-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




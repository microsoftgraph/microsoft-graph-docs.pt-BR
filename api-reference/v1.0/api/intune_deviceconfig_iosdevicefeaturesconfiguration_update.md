# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="6055b-101">Atualizar iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="6055b-101">Update iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="6055b-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6055b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6055b-103">Atualizar as propriedades de um objeto [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6055b-103">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6055b-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6055b-104">Prerequisites</span></span>
<span data-ttu-id="6055b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6055b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6055b-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6055b-107">Permission type</span></span>|<span data-ttu-id="6055b-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6055b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6055b-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6055b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6055b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6055b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6055b-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6055b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6055b-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6055b-112">Not supported.</span></span>|
|<span data-ttu-id="6055b-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6055b-113">Application</span></span>|<span data-ttu-id="6055b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6055b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6055b-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6055b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6055b-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6055b-116">Request headers</span></span>
|<span data-ttu-id="6055b-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6055b-117">Header</span></span>|<span data-ttu-id="6055b-118">Valor</span><span class="sxs-lookup"><span data-stu-id="6055b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6055b-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="6055b-119">Authorization</span></span>|<span data-ttu-id="6055b-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6055b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6055b-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6055b-121">Accept</span></span>|<span data-ttu-id="6055b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6055b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6055b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6055b-123">Request body</span></span>
<span data-ttu-id="6055b-124">No corpo da solicitação, forneça uma representação JSON do objeto [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6055b-124">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="6055b-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6055b-125">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="6055b-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6055b-126">Property</span></span>|<span data-ttu-id="6055b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6055b-127">Type</span></span>|<span data-ttu-id="6055b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6055b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6055b-129">id</span><span class="sxs-lookup"><span data-stu-id="6055b-129">id</span></span>|<span data-ttu-id="6055b-130">String</span><span class="sxs-lookup"><span data-stu-id="6055b-130">String</span></span>|<span data-ttu-id="6055b-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6055b-131">Key of the entity.</span></span> <span data-ttu-id="6055b-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6055b-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6055b-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6055b-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6055b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6055b-134">DateTimeOffset</span></span>|<span data-ttu-id="6055b-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6055b-135">DateTime the object was last modified.</span></span> <span data-ttu-id="6055b-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6055b-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6055b-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6055b-137">createdDateTime</span></span>|<span data-ttu-id="6055b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6055b-138">DateTimeOffset</span></span>|<span data-ttu-id="6055b-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6055b-139">DateTime the object was created.</span></span> <span data-ttu-id="6055b-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6055b-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6055b-141">descrição</span><span class="sxs-lookup"><span data-stu-id="6055b-141">description</span></span>|<span data-ttu-id="6055b-142">String</span><span class="sxs-lookup"><span data-stu-id="6055b-142">String</span></span>|<span data-ttu-id="6055b-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6055b-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6055b-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6055b-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6055b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="6055b-145">displayName</span></span>|<span data-ttu-id="6055b-146">String</span><span class="sxs-lookup"><span data-stu-id="6055b-146">String</span></span>|<span data-ttu-id="6055b-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6055b-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6055b-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6055b-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6055b-149">version</span><span class="sxs-lookup"><span data-stu-id="6055b-149">version</span></span>|<span data-ttu-id="6055b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6055b-150">Int32</span></span>|<span data-ttu-id="6055b-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6055b-151">Version of the device configuration.</span></span> <span data-ttu-id="6055b-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6055b-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6055b-153">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="6055b-153">assetTagTemplate</span></span>|<span data-ttu-id="6055b-154">String</span><span class="sxs-lookup"><span data-stu-id="6055b-154">String</span></span>|<span data-ttu-id="6055b-155">Informações de marcação de ativos para o dispositivo, exibidas na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="6055b-155">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="6055b-156">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="6055b-156">lockScreenFootnote</span></span>|<span data-ttu-id="6055b-157">String</span><span class="sxs-lookup"><span data-stu-id="6055b-157">String</span></span>|<span data-ttu-id="6055b-158">Uma nota de rodapé exibida na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="6055b-158">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="6055b-159">Disponível no iOS 9.3.1 e posterior.</span><span class="sxs-lookup"><span data-stu-id="6055b-159">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="6055b-160">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="6055b-160">homeScreenDockIcons</span></span>|<span data-ttu-id="6055b-161">Coleção [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="6055b-161">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="6055b-162">Uma lista dos aplicativos e pastas exibidos em um dock de tela inicial.</span><span class="sxs-lookup"><span data-stu-id="6055b-162">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="6055b-163">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6055b-163">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6055b-164">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="6055b-164">homeScreenPages</span></span>|<span data-ttu-id="6055b-165">Coleção [iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="6055b-165">[iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="6055b-166">Uma lista de páginas na tela inicial.</span><span class="sxs-lookup"><span data-stu-id="6055b-166">A list of pages on the Home Screen.</span></span> <span data-ttu-id="6055b-167">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6055b-167">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6055b-168">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="6055b-168">notificationSettings</span></span>|<span data-ttu-id="6055b-169">Coleção [iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6055b-169">[iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="6055b-170">Configurações de notificação para cada ID de pacote. Aplicáveis apenas a dispositivos no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="6055b-170">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="6055b-171">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6055b-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6055b-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="6055b-172">Response</span></span>
<span data-ttu-id="6055b-173">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6055b-173">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6055b-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6055b-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="6055b-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6055b-175">Request</span></span>
<span data-ttu-id="6055b-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6055b-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6055b-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="6055b-177">Response</span></span>
<span data-ttu-id="6055b-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6055b-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




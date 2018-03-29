# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="7003c-101">Atualizar iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="7003c-101">Update iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="7003c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7003c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7003c-103">Atualizar as propriedades de um objeto [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7003c-103">Update the properties of a [calendar](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7003c-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7003c-104">Prerequisites</span></span>
<span data-ttu-id="7003c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7003c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7003c-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7003c-107">Permission type</span></span>|<span data-ttu-id="7003c-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7003c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7003c-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7003c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7003c-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7003c-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7003c-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7003c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7003c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7003c-112">Not supported.</span></span>|
|<span data-ttu-id="7003c-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7003c-113">Application</span></span>|<span data-ttu-id="7003c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7003c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7003c-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7003c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7003c-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7003c-116">Request headers</span></span>
|<span data-ttu-id="7003c-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7003c-117">Header</span></span>|<span data-ttu-id="7003c-118">Valor</span><span class="sxs-lookup"><span data-stu-id="7003c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7003c-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="7003c-119">Authorization</span></span>|<span data-ttu-id="7003c-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7003c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7003c-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7003c-121">Accept</span></span>|<span data-ttu-id="7003c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7003c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7003c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7003c-123">Request body</span></span>
<span data-ttu-id="7003c-124">No corpo da solicitação, forneça uma representação JSON do objeto [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7003c-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="7003c-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7003c-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="7003c-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7003c-126">Property</span></span>|<span data-ttu-id="7003c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="7003c-127">Type</span></span>|<span data-ttu-id="7003c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7003c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7003c-129">id</span><span class="sxs-lookup"><span data-stu-id="7003c-129">id</span></span>|<span data-ttu-id="7003c-130">String</span><span class="sxs-lookup"><span data-stu-id="7003c-130">String</span></span>|<span data-ttu-id="7003c-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7003c-131">Key of the setting.</span></span> <span data-ttu-id="7003c-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7003c-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7003c-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7003c-133">lastModifiedDateTime</span></span>|<span data-ttu-id="7003c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7003c-134">DateTimeOffset</span></span>|<span data-ttu-id="7003c-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7003c-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="7003c-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7003c-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7003c-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7003c-137">createdDateTime</span></span>|<span data-ttu-id="7003c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7003c-138">DateTimeOffset</span></span>|<span data-ttu-id="7003c-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7003c-139">DateTime the object was created.</span></span> <span data-ttu-id="7003c-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7003c-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7003c-141">descrição</span><span class="sxs-lookup"><span data-stu-id="7003c-141">description</span></span>|<span data-ttu-id="7003c-142">String</span><span class="sxs-lookup"><span data-stu-id="7003c-142">String</span></span>|<span data-ttu-id="7003c-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7003c-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7003c-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7003c-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7003c-145">displayName</span><span class="sxs-lookup"><span data-stu-id="7003c-145">displayName</span></span>|<span data-ttu-id="7003c-146">String</span><span class="sxs-lookup"><span data-stu-id="7003c-146">String</span></span>|<span data-ttu-id="7003c-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7003c-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7003c-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7003c-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7003c-149">version</span><span class="sxs-lookup"><span data-stu-id="7003c-149">version</span></span>|<span data-ttu-id="7003c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7003c-150">Int32</span></span>|<span data-ttu-id="7003c-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7003c-151">Version of the device configuration.</span></span> <span data-ttu-id="7003c-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7003c-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7003c-153">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="7003c-153">assetTagTemplate</span></span>|<span data-ttu-id="7003c-154">String</span><span class="sxs-lookup"><span data-stu-id="7003c-154">String</span></span>|<span data-ttu-id="7003c-155">Informações de marcação de ativos para o dispositivo, exibidas na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="7003c-155">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="7003c-156">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="7003c-156">lockScreenFootnote</span></span>|<span data-ttu-id="7003c-157">String</span><span class="sxs-lookup"><span data-stu-id="7003c-157">String</span></span>|<span data-ttu-id="7003c-158">Uma nota de rodapé exibida na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="7003c-158">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="7003c-159">Disponível no iOS 9.3.1 e posterior.</span><span class="sxs-lookup"><span data-stu-id="7003c-159">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="7003c-160">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="7003c-160">homeScreenDockIcons</span></span>|<span data-ttu-id="7003c-161">Coleção [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="7003c-161">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="7003c-162">Uma lista dos aplicativos e pastas exibidos em um dock de tela inicial.</span><span class="sxs-lookup"><span data-stu-id="7003c-162">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="7003c-163">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="7003c-163">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7003c-164">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="7003c-164">homeScreenPages</span></span>|<span data-ttu-id="7003c-165">Coleção [iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="7003c-165">[iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="7003c-166">Uma lista de páginas na tela inicial.</span><span class="sxs-lookup"><span data-stu-id="7003c-166">A list of pages on the Home Screen.</span></span> <span data-ttu-id="7003c-167">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="7003c-167">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7003c-168">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="7003c-168">notificationSettings</span></span>|<span data-ttu-id="7003c-169">Coleção [iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="7003c-169">[iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="7003c-170">Configurações de notificação para cada ID de pacote. Aplicáveis apenas a dispositivos no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="7003c-170">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="7003c-171">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="7003c-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="7003c-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="7003c-172">Response</span></span>
<span data-ttu-id="7003c-173">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7003c-173">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7003c-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7003c-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="7003c-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7003c-175">Request</span></span>
<span data-ttu-id="7003c-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7003c-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1983

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="7003c-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="7003c-177">Response</span></span>
<span data-ttu-id="7003c-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7003c-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




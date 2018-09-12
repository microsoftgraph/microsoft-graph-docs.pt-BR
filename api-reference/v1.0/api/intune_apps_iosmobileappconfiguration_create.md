# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="f2e9b-101">Criar iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2e9b-101">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="f2e9b-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2e9b-103">Cria um novo objeto [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2e9b-103">Create a new [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f2e9b-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2e9b-104">Prerequisites</span></span>
<span data-ttu-id="f2e9b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f2e9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f2e9b-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2e9b-107">Permission type</span></span>|<span data-ttu-id="f2e9b-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2e9b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2e9b-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2e9b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f2e9b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2e9b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2e9b-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2e9b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2e9b-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-112">Not supported.</span></span>|
|<span data-ttu-id="f2e9b-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2e9b-113">Application</span></span>|<span data-ttu-id="f2e9b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2e9b-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2e9b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f2e9b-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2e9b-116">Request headers</span></span>
|<span data-ttu-id="f2e9b-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2e9b-117">Header</span></span>|<span data-ttu-id="f2e9b-118">Valor</span><span class="sxs-lookup"><span data-stu-id="f2e9b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2e9b-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2e9b-119">Authorization</span></span>|<span data-ttu-id="f2e9b-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="f2e9b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2e9b-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2e9b-121">Accept</span></span>|<span data-ttu-id="f2e9b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f2e9b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2e9b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2e9b-123">Request body</span></span>
<span data-ttu-id="f2e9b-124">No corpo da solicitação, forneça uma representação JSON do objeto iosMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-124">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="f2e9b-125">A tabela a seguir mostra as propriedades que são necessárias ao criar o iosMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-125">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="f2e9b-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2e9b-126">Property</span></span>|<span data-ttu-id="f2e9b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2e9b-127">Type</span></span>|<span data-ttu-id="f2e9b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2e9b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2e9b-129">id</span><span class="sxs-lookup"><span data-stu-id="f2e9b-129">id</span></span>|<span data-ttu-id="f2e9b-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2e9b-130">String</span></span>|<span data-ttu-id="f2e9b-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-131">Key of the entity.</span></span> <span data-ttu-id="f2e9b-132">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2e9b-132">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f2e9b-133">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="f2e9b-133">targetedMobileApps</span></span>|<span data-ttu-id="f2e9b-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2e9b-134">String collection</span></span>|<span data-ttu-id="f2e9b-135">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-135">the associated app.</span></span> <span data-ttu-id="f2e9b-136">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2e9b-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f2e9b-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2e9b-137">createdDateTime</span></span>|<span data-ttu-id="f2e9b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2e9b-138">DateTimeOffset</span></span>|<span data-ttu-id="f2e9b-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-139">DateTime the object was created.</span></span> <span data-ttu-id="f2e9b-140">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2e9b-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f2e9b-141">description</span><span class="sxs-lookup"><span data-stu-id="f2e9b-141">description</span></span>|<span data-ttu-id="f2e9b-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2e9b-142">String</span></span>|<span data-ttu-id="f2e9b-143">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f2e9b-144">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2e9b-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f2e9b-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2e9b-145">lastModifiedDateTime</span></span>|<span data-ttu-id="f2e9b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2e9b-146">DateTimeOffset</span></span>|<span data-ttu-id="f2e9b-147">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-147">DateTime the object was last modified.</span></span> <span data-ttu-id="f2e9b-148">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2e9b-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f2e9b-149">displayName</span><span class="sxs-lookup"><span data-stu-id="f2e9b-149">displayName</span></span>|<span data-ttu-id="f2e9b-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2e9b-150">String</span></span>|<span data-ttu-id="f2e9b-151">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-151">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f2e9b-152">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2e9b-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f2e9b-153">version</span><span class="sxs-lookup"><span data-stu-id="f2e9b-153">version</span></span>|<span data-ttu-id="f2e9b-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f2e9b-154">Int32</span></span>|<span data-ttu-id="f2e9b-155">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-155">Version of the device configuration.</span></span> <span data-ttu-id="f2e9b-156">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2e9b-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f2e9b-157">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="f2e9b-157">encodedSettingXml</span></span>|<span data-ttu-id="f2e9b-158">Binário</span><span class="sxs-lookup"><span data-stu-id="f2e9b-158">Binary</span></span>|<span data-ttu-id="f2e9b-159">Binário Base64 de configuração do aplicativo MDM.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-159">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="f2e9b-160">configurações</span><span class="sxs-lookup"><span data-stu-id="f2e9b-160">settings</span></span>|<span data-ttu-id="f2e9b-161">Coleção de [appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="f2e9b-161">[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="f2e9b-162">Itens de configuração de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-162">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="f2e9b-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2e9b-163">Response</span></span>
<span data-ttu-id="f2e9b-164">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-164">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2e9b-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2e9b-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="f2e9b-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2e9b-166">Request</span></span>
<span data-ttu-id="f2e9b-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 598

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
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

### <a name="response"></a><span data-ttu-id="f2e9b-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2e9b-168">Response</span></span>
<span data-ttu-id="f2e9b-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2e9b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









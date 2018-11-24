# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="9361d-101">Atualizar iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9361d-101">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="9361d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9361d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9361d-103">Atualiza as propriedades de um objeto [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9361d-103">Update the properties of a [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9361d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9361d-104">Prerequisites</span></span>
<span data-ttu-id="9361d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9361d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9361d-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9361d-107">Permission type</span></span>|<span data-ttu-id="9361d-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9361d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9361d-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9361d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9361d-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9361d-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9361d-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9361d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9361d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9361d-112">Not supported.</span></span>|
|<span data-ttu-id="9361d-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9361d-113">Application</span></span>|<span data-ttu-id="9361d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9361d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9361d-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9361d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9361d-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9361d-116">Request headers</span></span>
|<span data-ttu-id="9361d-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9361d-117">Header</span></span>|<span data-ttu-id="9361d-118">Valor</span><span class="sxs-lookup"><span data-stu-id="9361d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9361d-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="9361d-119">Authorization</span></span>|<span data-ttu-id="9361d-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9361d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9361d-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9361d-121">Accept</span></span>|<span data-ttu-id="9361d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9361d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9361d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9361d-123">Request body</span></span>
<span data-ttu-id="9361d-124">No corpo da solicitação, forneça uma representação JSON do objeto [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9361d-124">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="9361d-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9361d-125">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="9361d-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9361d-126">Property</span></span>|<span data-ttu-id="9361d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="9361d-127">Type</span></span>|<span data-ttu-id="9361d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9361d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9361d-129">id</span><span class="sxs-lookup"><span data-stu-id="9361d-129">id</span></span>|<span data-ttu-id="9361d-130">String</span><span class="sxs-lookup"><span data-stu-id="9361d-130">String</span></span>|<span data-ttu-id="9361d-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9361d-131">Key of the entity.</span></span> <span data-ttu-id="9361d-132">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9361d-132">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9361d-133">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="9361d-133">targetedMobileApps</span></span>|<span data-ttu-id="9361d-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9361d-134">String collection</span></span>|<span data-ttu-id="9361d-135">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="9361d-135">the associated app.</span></span> <span data-ttu-id="9361d-136">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9361d-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9361d-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9361d-137">createdDateTime</span></span>|<span data-ttu-id="9361d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9361d-138">DateTimeOffset</span></span>|<span data-ttu-id="9361d-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9361d-139">DateTime the object was created.</span></span> <span data-ttu-id="9361d-140">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9361d-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9361d-141">description</span><span class="sxs-lookup"><span data-stu-id="9361d-141">description</span></span>|<span data-ttu-id="9361d-142">String</span><span class="sxs-lookup"><span data-stu-id="9361d-142">String</span></span>|<span data-ttu-id="9361d-143">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9361d-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9361d-144">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9361d-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9361d-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9361d-145">lastModifiedDateTime</span></span>|<span data-ttu-id="9361d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9361d-146">DateTimeOffset</span></span>|<span data-ttu-id="9361d-147">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9361d-147">DateTime the object was last modified.</span></span> <span data-ttu-id="9361d-148">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9361d-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9361d-149">displayName</span><span class="sxs-lookup"><span data-stu-id="9361d-149">displayName</span></span>|<span data-ttu-id="9361d-150">String</span><span class="sxs-lookup"><span data-stu-id="9361d-150">String</span></span>|<span data-ttu-id="9361d-151">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9361d-151">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9361d-152">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9361d-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9361d-153">version</span><span class="sxs-lookup"><span data-stu-id="9361d-153">version</span></span>|<span data-ttu-id="9361d-154">Int32</span><span class="sxs-lookup"><span data-stu-id="9361d-154">Int32</span></span>|<span data-ttu-id="9361d-155">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9361d-155">Version of the device configuration.</span></span> <span data-ttu-id="9361d-156">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9361d-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9361d-157">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="9361d-157">encodedSettingXml</span></span>|<span data-ttu-id="9361d-158">Binário</span><span class="sxs-lookup"><span data-stu-id="9361d-158">Binary</span></span>|<span data-ttu-id="9361d-159">Binário Base64 de configuração do aplicativo MDM.</span><span class="sxs-lookup"><span data-stu-id="9361d-159">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="9361d-160">configurações</span><span class="sxs-lookup"><span data-stu-id="9361d-160">settings</span></span>|<span data-ttu-id="9361d-161">Coleção de [appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="9361d-161">[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="9361d-162">Itens de configuração de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9361d-162">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="9361d-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="9361d-163">Response</span></span>
<span data-ttu-id="9361d-164">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9361d-164">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9361d-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9361d-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="9361d-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9361d-166">Request</span></span>
<span data-ttu-id="9361d-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9361d-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9361d-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="9361d-168">Response</span></span>
<span data-ttu-id="9361d-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9361d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




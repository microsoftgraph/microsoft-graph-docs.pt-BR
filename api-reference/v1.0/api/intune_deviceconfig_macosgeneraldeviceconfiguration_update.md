# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="56aa5-101">Atualizar macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="56aa5-101">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="56aa5-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="56aa5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56aa5-103">Atualiza as propriedades de um objeto [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="56aa5-103">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56aa5-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="56aa5-104">Prerequisites</span></span>
<span data-ttu-id="56aa5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="56aa5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="56aa5-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56aa5-107">Permission type</span></span>|<span data-ttu-id="56aa5-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="56aa5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56aa5-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56aa5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="56aa5-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56aa5-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="56aa5-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56aa5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56aa5-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56aa5-112">Not supported.</span></span>|
|<span data-ttu-id="56aa5-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56aa5-113">Application</span></span>|<span data-ttu-id="56aa5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56aa5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56aa5-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56aa5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="56aa5-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56aa5-116">Request headers</span></span>
|<span data-ttu-id="56aa5-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56aa5-117">Header</span></span>|<span data-ttu-id="56aa5-118">Valor</span><span class="sxs-lookup"><span data-stu-id="56aa5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56aa5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="56aa5-119">Authorization</span></span>|<span data-ttu-id="56aa5-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56aa5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56aa5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="56aa5-121">Accept</span></span>|<span data-ttu-id="56aa5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="56aa5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56aa5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56aa5-123">Request body</span></span>
<span data-ttu-id="56aa5-124">No corpo da solicitação, forneça uma representação JSON do objeto [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="56aa5-124">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="56aa5-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="56aa5-125">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="56aa5-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56aa5-126">Property</span></span>|<span data-ttu-id="56aa5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="56aa5-127">Type</span></span>|<span data-ttu-id="56aa5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="56aa5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56aa5-129">id</span><span class="sxs-lookup"><span data-stu-id="56aa5-129">id</span></span>|<span data-ttu-id="56aa5-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56aa5-130">String</span></span>|<span data-ttu-id="56aa5-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="56aa5-131">Key of the entity.</span></span> <span data-ttu-id="56aa5-132">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56aa5-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56aa5-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56aa5-133">lastModifiedDateTime</span></span>|<span data-ttu-id="56aa5-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56aa5-134">DateTimeOffset</span></span>|<span data-ttu-id="56aa5-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="56aa5-135">DateTime the object was last modified.</span></span> <span data-ttu-id="56aa5-136">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56aa5-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56aa5-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56aa5-137">createdDateTime</span></span>|<span data-ttu-id="56aa5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56aa5-138">DateTimeOffset</span></span>|<span data-ttu-id="56aa5-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="56aa5-139">DateTime the object was created.</span></span> <span data-ttu-id="56aa5-140">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56aa5-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56aa5-141">description</span><span class="sxs-lookup"><span data-stu-id="56aa5-141">description</span></span>|<span data-ttu-id="56aa5-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56aa5-142">String</span></span>|<span data-ttu-id="56aa5-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="56aa5-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="56aa5-144">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56aa5-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56aa5-145">displayName</span><span class="sxs-lookup"><span data-stu-id="56aa5-145">displayName</span></span>|<span data-ttu-id="56aa5-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56aa5-146">String</span></span>|<span data-ttu-id="56aa5-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="56aa5-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="56aa5-148">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56aa5-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56aa5-149">version</span><span class="sxs-lookup"><span data-stu-id="56aa5-149">version</span></span>|<span data-ttu-id="56aa5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="56aa5-150">Int32</span></span>|<span data-ttu-id="56aa5-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="56aa5-151">Version of the device configuration.</span></span> <span data-ttu-id="56aa5-152">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56aa5-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56aa5-153">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="56aa5-153">compliantAppsList</span></span>|<span data-ttu-id="56aa5-154">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="56aa5-154">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="56aa5-155">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="56aa5-155">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="56aa5-156">Essa coleção pode conter um máximo de 10000 elementos.</span><span class="sxs-lookup"><span data-stu-id="56aa5-156">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="56aa5-157">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="56aa5-157">compliantAppListType</span></span>|[<span data-ttu-id="56aa5-158">appListType</span><span class="sxs-lookup"><span data-stu-id="56aa5-158">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="56aa5-159">Lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="56aa5-159">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="56aa5-160">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="56aa5-160">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="56aa5-161">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="56aa5-161">emailInDomainSuffixes</span></span>|<span data-ttu-id="56aa5-162">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56aa5-162">String collection</span></span>|<span data-ttu-id="56aa5-163">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="56aa5-163">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="56aa5-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="56aa5-164">passwordBlockSimple</span></span>|<span data-ttu-id="56aa5-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="56aa5-165">Boolean</span></span>|<span data-ttu-id="56aa5-166">Bloquear senhas simples.</span><span class="sxs-lookup"><span data-stu-id="56aa5-166">Block simple passwords.</span></span>|
|<span data-ttu-id="56aa5-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="56aa5-167">passwordExpirationDays</span></span>|<span data-ttu-id="56aa5-168">Int32</span><span class="sxs-lookup"><span data-stu-id="56aa5-168">Int32</span></span>|<span data-ttu-id="56aa5-169">Número de dias antes que a senha expire.</span><span class="sxs-lookup"><span data-stu-id="56aa5-169">Number of days before the password expires.</span></span>|
|<span data-ttu-id="56aa5-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="56aa5-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="56aa5-171">Int32</span><span class="sxs-lookup"><span data-stu-id="56aa5-171">Int32</span></span>|<span data-ttu-id="56aa5-172">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="56aa5-172">Number of character sets a password must contain.</span></span> <span data-ttu-id="56aa5-173">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="56aa5-173">Valid values 0 to 4</span></span>|
|<span data-ttu-id="56aa5-174">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="56aa5-174">passwordMinimumLength</span></span>|<span data-ttu-id="56aa5-175">Int32</span><span class="sxs-lookup"><span data-stu-id="56aa5-175">Int32</span></span>|<span data-ttu-id="56aa5-176">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="56aa5-176">Minimum length of passwords.</span></span>|
|<span data-ttu-id="56aa5-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="56aa5-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="56aa5-178">Int32</span><span class="sxs-lookup"><span data-stu-id="56aa5-178">Int32</span></span>|<span data-ttu-id="56aa5-179">Minutos de inatividade necessários antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="56aa5-179">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="56aa5-180">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="56aa5-180">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="56aa5-181">Int32</span><span class="sxs-lookup"><span data-stu-id="56aa5-181">Int32</span></span>|<span data-ttu-id="56aa5-182">Minutos de inatividade necessários antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="56aa5-182">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="56aa5-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="56aa5-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="56aa5-184">Int32</span><span class="sxs-lookup"><span data-stu-id="56aa5-184">Int32</span></span>|<span data-ttu-id="56aa5-185">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="56aa5-185">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="56aa5-186">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="56aa5-186">passwordRequiredType</span></span>|[<span data-ttu-id="56aa5-187">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="56aa5-187">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="56aa5-188">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="56aa5-188">Type of password that is required.</span></span> <span data-ttu-id="56aa5-189">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="56aa5-189">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="56aa5-190">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="56aa5-190">passwordRequired</span></span>|<span data-ttu-id="56aa5-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="56aa5-191">Boolean</span></span>|<span data-ttu-id="56aa5-192">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="56aa5-192">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="56aa5-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="56aa5-193">Response</span></span>
<span data-ttu-id="56aa5-194">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56aa5-194">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56aa5-195">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56aa5-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="56aa5-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56aa5-196">Request</span></span>
<span data-ttu-id="56aa5-197">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56aa5-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 906

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```

### <a name="response"></a><span data-ttu-id="56aa5-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="56aa5-198">Response</span></span>
<span data-ttu-id="56aa5-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56aa5-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1078

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```




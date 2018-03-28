# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="72fd2-101">Atualizar macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="72fd2-101">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="72fd2-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="72fd2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72fd2-103">Atualiza as propriedades de um objeto [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72fd2-103">Update the properties of a [calendar](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="72fd2-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72fd2-104">Prerequisites</span></span>
<span data-ttu-id="72fd2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="72fd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="72fd2-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72fd2-107">Permission type</span></span>|<span data-ttu-id="72fd2-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="72fd2-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72fd2-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72fd2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="72fd2-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72fd2-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72fd2-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72fd2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72fd2-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72fd2-112">Not supported.</span></span>|
|<span data-ttu-id="72fd2-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72fd2-113">Application</span></span>|<span data-ttu-id="72fd2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72fd2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72fd2-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72fd2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="72fd2-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72fd2-116">Request headers</span></span>
|<span data-ttu-id="72fd2-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72fd2-117">Header</span></span>|<span data-ttu-id="72fd2-118">Valor</span><span class="sxs-lookup"><span data-stu-id="72fd2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72fd2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="72fd2-119">Authorization</span></span>|<span data-ttu-id="72fd2-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72fd2-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="72fd2-121">Accept</span><span class="sxs-lookup"><span data-stu-id="72fd2-121">Accept</span></span>|<span data-ttu-id="72fd2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="72fd2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72fd2-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72fd2-123">Request body</span></span>
<span data-ttu-id="72fd2-124">No corpo da solicitação, forneça uma representação JSON do objeto [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72fd2-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="72fd2-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72fd2-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="72fd2-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72fd2-126">Property</span></span>|<span data-ttu-id="72fd2-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="72fd2-127">Type</span></span>|<span data-ttu-id="72fd2-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="72fd2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72fd2-129">id</span><span class="sxs-lookup"><span data-stu-id="72fd2-129">id</span></span>|<span data-ttu-id="72fd2-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72fd2-130">String</span></span>|<span data-ttu-id="72fd2-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="72fd2-131">Key of the setting.</span></span> <span data-ttu-id="72fd2-132">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72fd2-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72fd2-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72fd2-133">lastModifiedDateTime</span></span>|<span data-ttu-id="72fd2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72fd2-134">DateTimeOffset</span></span>|<span data-ttu-id="72fd2-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="72fd2-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="72fd2-136">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72fd2-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72fd2-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72fd2-137">createdDateTime</span></span>|<span data-ttu-id="72fd2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72fd2-138">DateTimeOffset</span></span>|<span data-ttu-id="72fd2-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="72fd2-139">DateTime the object was created.</span></span> <span data-ttu-id="72fd2-140">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72fd2-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72fd2-141">description</span><span class="sxs-lookup"><span data-stu-id="72fd2-141">description</span></span>|<span data-ttu-id="72fd2-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72fd2-142">String</span></span>|<span data-ttu-id="72fd2-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="72fd2-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="72fd2-144">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72fd2-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72fd2-145">displayName</span><span class="sxs-lookup"><span data-stu-id="72fd2-145">displayName</span></span>|<span data-ttu-id="72fd2-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72fd2-146">String</span></span>|<span data-ttu-id="72fd2-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="72fd2-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="72fd2-148">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72fd2-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72fd2-149">version</span><span class="sxs-lookup"><span data-stu-id="72fd2-149">version</span></span>|<span data-ttu-id="72fd2-150">Int32</span><span class="sxs-lookup"><span data-stu-id="72fd2-150">Int32</span></span>|<span data-ttu-id="72fd2-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="72fd2-151">Version of the device configuration.</span></span> <span data-ttu-id="72fd2-152">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72fd2-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72fd2-153">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="72fd2-153">compliantAppsList</span></span>|<span data-ttu-id="72fd2-154">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="72fd2-154">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="72fd2-155">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="72fd2-155">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="72fd2-156">Essa coleção pode conter um máximo de 10000 elementos.</span><span class="sxs-lookup"><span data-stu-id="72fd2-156">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="72fd2-157">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="72fd2-157">compliantAppListType</span></span>|<span data-ttu-id="72fd2-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72fd2-158">String</span></span>|<span data-ttu-id="72fd2-159">Lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="72fd2-159">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="72fd2-160">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="72fd2-160">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="72fd2-161">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="72fd2-161">emailInDomainSuffixes</span></span>|<span data-ttu-id="72fd2-162">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72fd2-162">String collection</span></span>|<span data-ttu-id="72fd2-163">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="72fd2-163">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="72fd2-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="72fd2-164">passwordBlockSimple</span></span>|<span data-ttu-id="72fd2-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="72fd2-165">Boolean</span></span>|<span data-ttu-id="72fd2-166">Bloquear senhas simples.</span><span class="sxs-lookup"><span data-stu-id="72fd2-166">Block simple passwords.</span></span>|
|<span data-ttu-id="72fd2-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="72fd2-167">passwordExpirationDays</span></span>|<span data-ttu-id="72fd2-168">Int32</span><span class="sxs-lookup"><span data-stu-id="72fd2-168">Int32</span></span>|<span data-ttu-id="72fd2-169">Número de dias antes que a senha expire.</span><span class="sxs-lookup"><span data-stu-id="72fd2-169">Number of days before the password expires.</span></span>|
|<span data-ttu-id="72fd2-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="72fd2-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="72fd2-171">Int32</span><span class="sxs-lookup"><span data-stu-id="72fd2-171">Int32</span></span>|<span data-ttu-id="72fd2-172">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="72fd2-172">Number of character sets a password must contain.</span></span> <span data-ttu-id="72fd2-173">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="72fd2-173">Valid values 0 to 4</span></span>|
|<span data-ttu-id="72fd2-174">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="72fd2-174">passwordMinimumLength</span></span>|<span data-ttu-id="72fd2-175">Int32</span><span class="sxs-lookup"><span data-stu-id="72fd2-175">Int32</span></span>|<span data-ttu-id="72fd2-176">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="72fd2-176">Minimum length of passwords.</span></span>|
|<span data-ttu-id="72fd2-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="72fd2-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="72fd2-178">Int32</span><span class="sxs-lookup"><span data-stu-id="72fd2-178">Int32</span></span>|<span data-ttu-id="72fd2-179">Minutos de inatividade necessários antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="72fd2-179">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="72fd2-180">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="72fd2-180">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="72fd2-181">Int32</span><span class="sxs-lookup"><span data-stu-id="72fd2-181">Int32</span></span>|<span data-ttu-id="72fd2-182">Minutos de inatividade necessários antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="72fd2-182">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="72fd2-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="72fd2-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="72fd2-184">Int32</span><span class="sxs-lookup"><span data-stu-id="72fd2-184">Int32</span></span>|<span data-ttu-id="72fd2-185">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="72fd2-185">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="72fd2-186">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="72fd2-186">passwordRequiredType</span></span>|<span data-ttu-id="72fd2-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72fd2-187">String</span></span>|<span data-ttu-id="72fd2-188">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="72fd2-188">Type of password that is required.</span></span> <span data-ttu-id="72fd2-189">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="72fd2-189">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="72fd2-190">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="72fd2-190">passwordRequired</span></span>|<span data-ttu-id="72fd2-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="72fd2-191">Boolean</span></span>|<span data-ttu-id="72fd2-192">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="72fd2-192">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="72fd2-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="72fd2-193">Response</span></span>
<span data-ttu-id="72fd2-194">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72fd2-194">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72fd2-195">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72fd2-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="72fd2-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72fd2-196">Request</span></span>
<span data-ttu-id="72fd2-197">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72fd2-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 900

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="72fd2-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="72fd2-198">Response</span></span>
<span data-ttu-id="72fd2-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72fd2-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




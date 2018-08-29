# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="f555d-101">Criar macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f555d-101">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="f555d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f555d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f555d-103">Cria um novo objeto [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f555d-103">Create a new [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f555d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f555d-104">Prerequisites</span></span>
<span data-ttu-id="f555d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f555d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f555d-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f555d-107">Permission type</span></span>|<span data-ttu-id="f555d-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f555d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f555d-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f555d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f555d-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f555d-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f555d-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f555d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f555d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f555d-112">Not supported.</span></span>|
|<span data-ttu-id="f555d-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f555d-113">Application</span></span>|<span data-ttu-id="f555d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f555d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f555d-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f555d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f555d-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f555d-116">Request headers</span></span>
|<span data-ttu-id="f555d-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f555d-117">Header</span></span>|<span data-ttu-id="f555d-118">Valor</span><span class="sxs-lookup"><span data-stu-id="f555d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f555d-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="f555d-119">Authorization</span></span>|<span data-ttu-id="f555d-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="f555d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f555d-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f555d-121">Accept</span></span>|<span data-ttu-id="f555d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f555d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f555d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f555d-123">Request body</span></span>
<span data-ttu-id="f555d-124">No corpo da solicitação, forneça uma representação JSON do objeto macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f555d-124">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="f555d-125">A tabela a seguir mostra as propriedades obrigatórias ao criar macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f555d-125">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="f555d-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f555d-126">Property</span></span>|<span data-ttu-id="f555d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f555d-127">Type</span></span>|<span data-ttu-id="f555d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f555d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f555d-129">id</span><span class="sxs-lookup"><span data-stu-id="f555d-129">id</span></span>|<span data-ttu-id="f555d-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f555d-130">String</span></span>|<span data-ttu-id="f555d-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f555d-131">Key of the entity.</span></span> <span data-ttu-id="f555d-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f555d-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f555d-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f555d-133">lastModifiedDateTime</span></span>|<span data-ttu-id="f555d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f555d-134">DateTimeOffset</span></span>|<span data-ttu-id="f555d-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f555d-135">DateTime the object was last modified.</span></span> <span data-ttu-id="f555d-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f555d-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f555d-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f555d-137">createdDateTime</span></span>|<span data-ttu-id="f555d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f555d-138">DateTimeOffset</span></span>|<span data-ttu-id="f555d-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f555d-139">DateTime the object was created.</span></span> <span data-ttu-id="f555d-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f555d-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f555d-141">description</span><span class="sxs-lookup"><span data-stu-id="f555d-141">description</span></span>|<span data-ttu-id="f555d-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f555d-142">String</span></span>|<span data-ttu-id="f555d-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f555d-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f555d-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f555d-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f555d-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f555d-145">displayName</span></span>|<span data-ttu-id="f555d-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f555d-146">String</span></span>|<span data-ttu-id="f555d-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f555d-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f555d-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f555d-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f555d-149">version</span><span class="sxs-lookup"><span data-stu-id="f555d-149">version</span></span>|<span data-ttu-id="f555d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f555d-150">Int32</span></span>|<span data-ttu-id="f555d-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f555d-151">Version of the device configuration.</span></span> <span data-ttu-id="f555d-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f555d-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f555d-153">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="f555d-153">compliantAppsList</span></span>|<span data-ttu-id="f555d-154">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="f555d-154">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="f555d-155">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="f555d-155">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="f555d-156">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="f555d-156">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="f555d-157">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="f555d-157">compliantAppListType</span></span>|[<span data-ttu-id="f555d-158">appListType</span><span class="sxs-lookup"><span data-stu-id="f555d-158">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="f555d-159">Lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="f555d-159">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="f555d-160">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="f555d-160">The possible values are:</span></span>|
|<span data-ttu-id="f555d-161">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="f555d-161">emailInDomainSuffixes</span></span>|<span data-ttu-id="f555d-162">Coleção de sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="f555d-162">String collection</span></span>|<span data-ttu-id="f555d-163">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="f555d-163">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="f555d-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f555d-164">passwordBlockSimple</span></span>|<span data-ttu-id="f555d-165">Booleano</span><span class="sxs-lookup"><span data-stu-id="f555d-165">Boolean</span></span>|<span data-ttu-id="f555d-166">Bloquear senhas simples.</span><span class="sxs-lookup"><span data-stu-id="f555d-166">Block simple passwords.</span></span>|
|<span data-ttu-id="f555d-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f555d-167">passwordExpirationDays</span></span>|<span data-ttu-id="f555d-168">Int32</span><span class="sxs-lookup"><span data-stu-id="f555d-168">Int32</span></span>|<span data-ttu-id="f555d-169">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="f555d-169">Number of days before the password expires.</span></span>|
|<span data-ttu-id="f555d-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f555d-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f555d-171">Int32</span><span class="sxs-lookup"><span data-stu-id="f555d-171">Int32</span></span>|<span data-ttu-id="f555d-172">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="f555d-172">Number of character sets a password must contain.</span></span> <span data-ttu-id="f555d-173">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="f555d-173">Valid values 0 to 4</span></span>|
|<span data-ttu-id="f555d-174">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f555d-174">passwordMinimumLength</span></span>|<span data-ttu-id="f555d-175">Int32</span><span class="sxs-lookup"><span data-stu-id="f555d-175">Int32</span></span>|<span data-ttu-id="f555d-176">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="f555d-176">Minimum length of passwords.</span></span>|
|<span data-ttu-id="f555d-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f555d-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f555d-178">Int32</span><span class="sxs-lookup"><span data-stu-id="f555d-178">Int32</span></span>|<span data-ttu-id="f555d-179">Minutos de inatividade necessários antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="f555d-179">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="f555d-180">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f555d-180">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f555d-181">Int32</span><span class="sxs-lookup"><span data-stu-id="f555d-181">Int32</span></span>|<span data-ttu-id="f555d-182">Minutos de inatividade necessários antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="f555d-182">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="f555d-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f555d-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f555d-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f555d-184">Int32</span></span>|<span data-ttu-id="f555d-185">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="f555d-185">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="f555d-186">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f555d-186">passwordRequiredType</span></span>|[<span data-ttu-id="f555d-187">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f555d-187">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="f555d-188">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="f555d-188">Type of password that is required.</span></span> <span data-ttu-id="f555d-189">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="f555d-189">The possible values are:</span></span>|
|<span data-ttu-id="f555d-190">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f555d-190">passwordRequired</span></span>|<span data-ttu-id="f555d-191">Booleano</span><span class="sxs-lookup"><span data-stu-id="f555d-191">Boolean</span></span>|<span data-ttu-id="f555d-192">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="f555d-192">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="f555d-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="f555d-193">Response</span></span>
<span data-ttu-id="f555d-194">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f555d-194">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f555d-195">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f555d-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="f555d-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f555d-196">Request</span></span>
<span data-ttu-id="f555d-197">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f555d-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 970

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="f555d-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="f555d-198">Response</span></span>
<span data-ttu-id="f555d-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f555d-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




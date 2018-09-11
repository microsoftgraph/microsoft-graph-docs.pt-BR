# <a name="create-managediosstoreapp"></a><span data-ttu-id="4ff43-101">Criar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="4ff43-101">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="4ff43-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4ff43-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ff43-103">Cria um novo objeto [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4ff43-103">Create a new [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ff43-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ff43-104">Prerequisites</span></span>
<span data-ttu-id="4ff43-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4ff43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4ff43-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ff43-107">Permission type</span></span>|<span data-ttu-id="4ff43-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4ff43-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ff43-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ff43-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4ff43-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ff43-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4ff43-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ff43-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ff43-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ff43-112">Not supported.</span></span>|
|<span data-ttu-id="4ff43-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ff43-113">Application</span></span>|<span data-ttu-id="4ff43-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ff43-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ff43-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ff43-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4ff43-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ff43-116">Request headers</span></span>
|<span data-ttu-id="4ff43-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ff43-117">Header</span></span>|<span data-ttu-id="4ff43-118">Valor</span><span class="sxs-lookup"><span data-stu-id="4ff43-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ff43-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ff43-119">Authorization</span></span>|<span data-ttu-id="4ff43-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="4ff43-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ff43-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4ff43-121">Accept</span></span>|<span data-ttu-id="4ff43-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4ff43-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ff43-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ff43-123">Request body</span></span>
<span data-ttu-id="4ff43-124">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="4ff43-124">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="4ff43-125">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="4ff43-125">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="4ff43-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ff43-126">Property</span></span>|<span data-ttu-id="4ff43-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ff43-127">Type</span></span>|<span data-ttu-id="4ff43-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ff43-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ff43-129">id</span><span class="sxs-lookup"><span data-stu-id="4ff43-129">id</span></span>|<span data-ttu-id="4ff43-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ff43-130">String</span></span>|<span data-ttu-id="4ff43-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4ff43-131">Key of the entity.</span></span> <span data-ttu-id="4ff43-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4ff43-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4ff43-133">displayName</span><span class="sxs-lookup"><span data-stu-id="4ff43-133">displayName</span></span>|<span data-ttu-id="4ff43-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ff43-134">String</span></span>|<span data-ttu-id="4ff43-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="4ff43-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4ff43-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4ff43-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4ff43-137">description</span><span class="sxs-lookup"><span data-stu-id="4ff43-137">description</span></span>|<span data-ttu-id="4ff43-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ff43-138">String</span></span>|<span data-ttu-id="4ff43-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4ff43-139">The description of the app.</span></span> <span data-ttu-id="4ff43-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4ff43-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4ff43-141">publisher</span><span class="sxs-lookup"><span data-stu-id="4ff43-141">publisher</span></span>|<span data-ttu-id="4ff43-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ff43-142">String</span></span>|<span data-ttu-id="4ff43-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4ff43-143">The publisher of the app.</span></span> <span data-ttu-id="4ff43-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4ff43-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4ff43-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4ff43-145">largeIcon</span></span>|[<span data-ttu-id="4ff43-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4ff43-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="4ff43-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="4ff43-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4ff43-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4ff43-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4ff43-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ff43-149">createdDateTime</span></span>|<span data-ttu-id="4ff43-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ff43-150">DateTimeOffset</span></span>|<span data-ttu-id="4ff43-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4ff43-151">The date and time the app was created.</span></span> <span data-ttu-id="4ff43-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4ff43-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4ff43-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ff43-153">lastModifiedDateTime</span></span>|<span data-ttu-id="4ff43-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ff43-154">DateTimeOffset</span></span>|<span data-ttu-id="4ff43-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4ff43-155">The date and time the app was last modified.</span></span> <span data-ttu-id="4ff43-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4ff43-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4ff43-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4ff43-157">isFeatured</span></span>|<span data-ttu-id="4ff43-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="4ff43-158">Boolean</span></span>|<span data-ttu-id="4ff43-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4ff43-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4ff43-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4ff43-160">privacyInformationUrl</span></span>|<span data-ttu-id="4ff43-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ff43-161">String</span></span>|<span data-ttu-id="4ff43-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4ff43-162">The privacy statement Url.</span></span> <span data-ttu-id="4ff43-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4ff43-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4ff43-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4ff43-164">informationUrl</span></span>|<span data-ttu-id="4ff43-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ff43-165">String</span></span>|<span data-ttu-id="4ff43-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="4ff43-166">The more information Url.</span></span> <span data-ttu-id="4ff43-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4ff43-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4ff43-168">owner</span><span class="sxs-lookup"><span data-stu-id="4ff43-168">owner</span></span>|<span data-ttu-id="4ff43-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ff43-169">String</span></span>|<span data-ttu-id="4ff43-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4ff43-170">The owner of the app.</span></span> <span data-ttu-id="4ff43-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4ff43-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4ff43-172">developer</span><span class="sxs-lookup"><span data-stu-id="4ff43-172">developer</span></span>|<span data-ttu-id="4ff43-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ff43-173">String</span></span>|<span data-ttu-id="4ff43-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4ff43-174">The developer of the app.</span></span> <span data-ttu-id="4ff43-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4ff43-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4ff43-176">Observações</span><span class="sxs-lookup"><span data-stu-id="4ff43-176">notes</span></span>|<span data-ttu-id="4ff43-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ff43-177">String</span></span>|<span data-ttu-id="4ff43-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4ff43-178">Notes for the app.</span></span> <span data-ttu-id="4ff43-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4ff43-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4ff43-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="4ff43-180">publishingState</span></span>|[<span data-ttu-id="4ff43-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4ff43-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="4ff43-p114">O estado de publicação do aplicativo. O aplicativo não pode ser atribuído a menos que esteja publicado. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4ff43-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4ff43-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="4ff43-186">appAvailability</span></span>|[<span data-ttu-id="4ff43-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="4ff43-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="4ff43-p115">A disponibilidade do aplicativo. Herdada de [managedApp](../resources/intune_apps_managedapp.md). Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="4ff43-p115">The Application's availability. Inherited from [managedApp](../resources/intune_apps_managedapp.md). The possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="4ff43-191">version</span><span class="sxs-lookup"><span data-stu-id="4ff43-191">version</span></span>|<span data-ttu-id="4ff43-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ff43-192">String</span></span>|<span data-ttu-id="4ff43-193">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4ff43-193">The Application's version.</span></span> <span data-ttu-id="4ff43-194">Herdado de [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="4ff43-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="4ff43-195">bundleId</span><span class="sxs-lookup"><span data-stu-id="4ff43-195">bundleId</span></span>|<span data-ttu-id="4ff43-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ff43-196">String</span></span>|<span data-ttu-id="4ff43-197">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="4ff43-197">The app's Bundle ID.</span></span>|
|<span data-ttu-id="4ff43-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4ff43-198">appStoreUrl</span></span>|<span data-ttu-id="4ff43-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ff43-199">String</span></span>|<span data-ttu-id="4ff43-200">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="4ff43-200">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="4ff43-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="4ff43-201">applicableDeviceType</span></span>|[<span data-ttu-id="4ff43-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="4ff43-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="4ff43-203">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="4ff43-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="4ff43-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4ff43-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4ff43-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4ff43-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="4ff43-206">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="4ff43-206">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="4ff43-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ff43-207">Response</span></span>
<span data-ttu-id="4ff43-208">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ff43-208">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ff43-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ff43-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ff43-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ff43-210">Request</span></span>
<span data-ttu-id="4ff43-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ff43-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1128

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="4ff43-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ff43-212">Response</span></span>
<span data-ttu-id="4ff43-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ff43-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1236

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```









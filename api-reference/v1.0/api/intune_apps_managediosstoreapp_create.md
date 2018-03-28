# <a name="create-managediosstoreapp"></a><span data-ttu-id="59bed-101">Criar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="59bed-101">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="59bed-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="59bed-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59bed-103">Cria um novo objeto [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="59bed-103">Create a new [plannerBucket](../resources/intune_apps_managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="59bed-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59bed-104">Prerequisites</span></span>
<span data-ttu-id="59bed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="59bed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="59bed-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59bed-107">Permission type</span></span>|<span data-ttu-id="59bed-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="59bed-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59bed-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59bed-109">Delegated (work or school account)</span></span>|<span data-ttu-id="59bed-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59bed-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="59bed-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59bed-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59bed-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59bed-112">Not supported.</span></span>|
|<span data-ttu-id="59bed-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59bed-113">Application</span></span>|<span data-ttu-id="59bed-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59bed-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59bed-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59bed-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="59bed-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59bed-116">Request headers</span></span>
|<span data-ttu-id="59bed-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59bed-117">Header</span></span>|<span data-ttu-id="59bed-118">Valor</span><span class="sxs-lookup"><span data-stu-id="59bed-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59bed-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="59bed-119">Authorization</span></span>|<span data-ttu-id="59bed-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59bed-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="59bed-121">Accept</span><span class="sxs-lookup"><span data-stu-id="59bed-121">Accept</span></span>|<span data-ttu-id="59bed-122">application/json</span><span class="sxs-lookup"><span data-stu-id="59bed-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59bed-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59bed-123">Request body</span></span>
<span data-ttu-id="59bed-124">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="59bed-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="59bed-125">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="59bed-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="59bed-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59bed-126">Property</span></span>|<span data-ttu-id="59bed-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="59bed-127">Type</span></span>|<span data-ttu-id="59bed-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="59bed-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59bed-129">id</span><span class="sxs-lookup"><span data-stu-id="59bed-129">id</span></span>|<span data-ttu-id="59bed-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59bed-130">String</span></span>|<span data-ttu-id="59bed-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="59bed-131">Key of the setting.</span></span> <span data-ttu-id="59bed-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59bed-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59bed-133">displayName</span><span class="sxs-lookup"><span data-stu-id="59bed-133">displayName</span></span>|<span data-ttu-id="59bed-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59bed-134">String</span></span>|<span data-ttu-id="59bed-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="59bed-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="59bed-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59bed-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59bed-137">description</span><span class="sxs-lookup"><span data-stu-id="59bed-137">description</span></span>|<span data-ttu-id="59bed-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59bed-138">String</span></span>|<span data-ttu-id="59bed-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59bed-139">The description of the app.</span></span> <span data-ttu-id="59bed-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59bed-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59bed-141">publisher</span><span class="sxs-lookup"><span data-stu-id="59bed-141">Publisher</span></span>|<span data-ttu-id="59bed-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59bed-142">String</span></span>|<span data-ttu-id="59bed-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59bed-143">The publisher of the app.</span></span> <span data-ttu-id="59bed-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59bed-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59bed-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="59bed-145">largeIcon</span></span>|[<span data-ttu-id="59bed-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="59bed-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="59bed-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="59bed-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="59bed-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59bed-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59bed-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59bed-149">createdDateTime</span></span>|<span data-ttu-id="59bed-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59bed-150">DateTimeOffset</span></span>|<span data-ttu-id="59bed-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59bed-151">The date and time the group was created.</span></span> <span data-ttu-id="59bed-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59bed-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59bed-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59bed-153">lastModifiedDateTime</span></span>|<span data-ttu-id="59bed-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59bed-154">DateTimeOffset</span></span>|<span data-ttu-id="59bed-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="59bed-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="59bed-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59bed-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59bed-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="59bed-157">isFeatured</span></span>|<span data-ttu-id="59bed-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="59bed-158">Boolean</span></span>|<span data-ttu-id="59bed-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59bed-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59bed-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="59bed-160">privacyInformationUrl</span></span>|<span data-ttu-id="59bed-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59bed-161">String</span></span>|<span data-ttu-id="59bed-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="59bed-162">The privacy statement Url.</span></span> <span data-ttu-id="59bed-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59bed-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59bed-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="59bed-164">informationUrl</span></span>|<span data-ttu-id="59bed-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59bed-165">String</span></span>|<span data-ttu-id="59bed-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="59bed-166">The more information Url.</span></span> <span data-ttu-id="59bed-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59bed-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59bed-168">owner</span><span class="sxs-lookup"><span data-stu-id="59bed-168">owner</span></span>|<span data-ttu-id="59bed-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59bed-169">String</span></span>|<span data-ttu-id="59bed-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="59bed-170">The owner of the app.</span></span> <span data-ttu-id="59bed-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59bed-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59bed-172">developer</span><span class="sxs-lookup"><span data-stu-id="59bed-172">"developer"</span></span>|<span data-ttu-id="59bed-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59bed-173">String</span></span>|<span data-ttu-id="59bed-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59bed-174">The developer of the app.</span></span> <span data-ttu-id="59bed-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59bed-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59bed-176">notes</span><span class="sxs-lookup"><span data-stu-id="59bed-176">Notes</span></span>|<span data-ttu-id="59bed-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59bed-177">String</span></span>|<span data-ttu-id="59bed-178">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59bed-178">Notes for the app.</span></span> <span data-ttu-id="59bed-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59bed-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59bed-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="59bed-180">publishingState</span></span>|<span data-ttu-id="59bed-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59bed-181">String</span></span>|<span data-ttu-id="59bed-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59bed-182">The publishing state for the app.</span></span> <span data-ttu-id="59bed-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="59bed-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="59bed-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os possíveis valores são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="59bed-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="59bed-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="59bed-185">appAvailability</span></span>|<span data-ttu-id="59bed-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59bed-186">String</span></span>|<span data-ttu-id="59bed-187">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59bed-187">The Application's availability.</span></span> <span data-ttu-id="59bed-188">Herdado de [managedApp](../resources/intune_apps_managedapp.md). Os possíveis valores são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="59bed-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="59bed-189">version</span><span class="sxs-lookup"><span data-stu-id="59bed-189">version</span></span>|<span data-ttu-id="59bed-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59bed-190">String</span></span>|<span data-ttu-id="59bed-191">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59bed-191">The Application's version.</span></span> <span data-ttu-id="59bed-192">Herdado de [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="59bed-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="59bed-193">bundleId</span><span class="sxs-lookup"><span data-stu-id="59bed-193">bundleId</span></span>|<span data-ttu-id="59bed-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59bed-194">String</span></span>|<span data-ttu-id="59bed-195">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="59bed-195">The app's Bundle ID.</span></span>|
|<span data-ttu-id="59bed-196">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="59bed-196">appStoreUrl</span></span>|<span data-ttu-id="59bed-197">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59bed-197">String</span></span>|<span data-ttu-id="59bed-198">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="59bed-198">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="59bed-199">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="59bed-199">applicableDeviceType</span></span>|[<span data-ttu-id="59bed-200">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="59bed-200">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="59bed-201">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="59bed-201">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="59bed-202">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="59bed-202">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="59bed-203">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="59bed-203">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="59bed-204">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="59bed-204">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="59bed-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="59bed-205">Response</span></span>
<span data-ttu-id="59bed-206">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59bed-206">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_apps_managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59bed-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59bed-207">Example</span></span>
### <a name="request"></a><span data-ttu-id="59bed-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59bed-208">Request</span></span>
<span data-ttu-id="59bed-209">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59bed-209">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="59bed-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="59bed-210">Response</span></span>
<span data-ttu-id="59bed-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59bed-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




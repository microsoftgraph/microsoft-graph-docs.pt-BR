# <a name="update-managediosstoreapp"></a><span data-ttu-id="fd821-101">Atualizar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="fd821-101">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="fd821-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fd821-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd821-103">Atualiza as propriedades de um objeto [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="fd821-103">Update the properties of a [calendar](../resources/intune_apps_managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd821-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd821-104">Prerequisites</span></span>
<span data-ttu-id="fd821-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd821-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fd821-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd821-107">Permission type</span></span>|<span data-ttu-id="fd821-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fd821-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd821-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd821-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fd821-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd821-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fd821-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd821-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd821-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd821-112">Not supported.</span></span>|
|<span data-ttu-id="fd821-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd821-113">Application</span></span>|<span data-ttu-id="fd821-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd821-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd821-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd821-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="fd821-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd821-116">Request headers</span></span>
|<span data-ttu-id="fd821-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd821-117">Header</span></span>|<span data-ttu-id="fd821-118">Valor</span><span class="sxs-lookup"><span data-stu-id="fd821-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd821-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd821-119">Authorization</span></span>|<span data-ttu-id="fd821-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd821-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fd821-121">Accept</span><span class="sxs-lookup"><span data-stu-id="fd821-121">Accept</span></span>|<span data-ttu-id="fd821-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fd821-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd821-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd821-123">Request body</span></span>
<span data-ttu-id="fd821-124">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="fd821-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_managediosstoreapp.md) object.</span></span>

<span data-ttu-id="fd821-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="fd821-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="fd821-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd821-126">Property</span></span>|<span data-ttu-id="fd821-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd821-127">Type</span></span>|<span data-ttu-id="fd821-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd821-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd821-129">id</span><span class="sxs-lookup"><span data-stu-id="fd821-129">id</span></span>|<span data-ttu-id="fd821-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd821-130">String</span></span>|<span data-ttu-id="fd821-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fd821-131">Key of the setting.</span></span> <span data-ttu-id="fd821-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd821-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd821-133">displayName</span><span class="sxs-lookup"><span data-stu-id="fd821-133">displayName</span></span>|<span data-ttu-id="fd821-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd821-134">String</span></span>|<span data-ttu-id="fd821-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="fd821-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fd821-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd821-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd821-137">description</span><span class="sxs-lookup"><span data-stu-id="fd821-137">description</span></span>|<span data-ttu-id="fd821-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd821-138">String</span></span>|<span data-ttu-id="fd821-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd821-139">The description of the app.</span></span> <span data-ttu-id="fd821-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd821-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd821-141">publisher</span><span class="sxs-lookup"><span data-stu-id="fd821-141">Publisher</span></span>|<span data-ttu-id="fd821-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd821-142">String</span></span>|<span data-ttu-id="fd821-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd821-143">The publisher of the app.</span></span> <span data-ttu-id="fd821-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd821-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd821-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fd821-145">largeIcon</span></span>|[<span data-ttu-id="fd821-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fd821-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="fd821-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="fd821-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fd821-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd821-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd821-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd821-149">createdDateTime</span></span>|<span data-ttu-id="fd821-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd821-150">DateTimeOffset</span></span>|<span data-ttu-id="fd821-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd821-151">The date and time the group was created.</span></span> <span data-ttu-id="fd821-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd821-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd821-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd821-153">lastModifiedDateTime</span></span>|<span data-ttu-id="fd821-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd821-154">DateTimeOffset</span></span>|<span data-ttu-id="fd821-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fd821-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="fd821-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd821-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd821-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fd821-157">isFeatured</span></span>|<span data-ttu-id="fd821-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="fd821-158">Boolean</span></span>|<span data-ttu-id="fd821-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd821-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd821-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fd821-160">privacyInformationUrl</span></span>|<span data-ttu-id="fd821-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd821-161">String</span></span>|<span data-ttu-id="fd821-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="fd821-162">The privacy statement Url.</span></span> <span data-ttu-id="fd821-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd821-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd821-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fd821-164">informationUrl</span></span>|<span data-ttu-id="fd821-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd821-165">String</span></span>|<span data-ttu-id="fd821-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="fd821-166">The more information Url.</span></span> <span data-ttu-id="fd821-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd821-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd821-168">owner</span><span class="sxs-lookup"><span data-stu-id="fd821-168">owner</span></span>|<span data-ttu-id="fd821-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd821-169">String</span></span>|<span data-ttu-id="fd821-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="fd821-170">The owner of the app.</span></span> <span data-ttu-id="fd821-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd821-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd821-172">developer</span><span class="sxs-lookup"><span data-stu-id="fd821-172">"developer"</span></span>|<span data-ttu-id="fd821-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd821-173">String</span></span>|<span data-ttu-id="fd821-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd821-174">The developer of the app.</span></span> <span data-ttu-id="fd821-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd821-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd821-176">notes</span><span class="sxs-lookup"><span data-stu-id="fd821-176">Notes</span></span>|<span data-ttu-id="fd821-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd821-177">String</span></span>|<span data-ttu-id="fd821-178">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd821-178">Notes for the app.</span></span> <span data-ttu-id="fd821-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd821-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd821-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="fd821-180">publishingState</span></span>|<span data-ttu-id="fd821-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd821-181">String</span></span>|<span data-ttu-id="fd821-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd821-182">The publishing state for the app.</span></span> <span data-ttu-id="fd821-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="fd821-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fd821-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os possíveis valores são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="fd821-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fd821-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="fd821-185">appAvailability</span></span>|<span data-ttu-id="fd821-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd821-186">String</span></span>|<span data-ttu-id="fd821-187">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd821-187">The Application's availability.</span></span> <span data-ttu-id="fd821-188">Herdado de [managedApp](../resources/intune_apps_managedapp.md). Os possíveis valores são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="fd821-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="fd821-189">version</span><span class="sxs-lookup"><span data-stu-id="fd821-189">version</span></span>|<span data-ttu-id="fd821-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd821-190">String</span></span>|<span data-ttu-id="fd821-191">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd821-191">The Application's version.</span></span> <span data-ttu-id="fd821-192">Herdado de [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd821-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="fd821-193">bundleId</span><span class="sxs-lookup"><span data-stu-id="fd821-193">bundleId</span></span>|<span data-ttu-id="fd821-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd821-194">String</span></span>|<span data-ttu-id="fd821-195">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="fd821-195">The app's Bundle ID.</span></span>|
|<span data-ttu-id="fd821-196">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="fd821-196">appStoreUrl</span></span>|<span data-ttu-id="fd821-197">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd821-197">String</span></span>|<span data-ttu-id="fd821-198">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="fd821-198">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="fd821-199">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="fd821-199">applicableDeviceType</span></span>|[<span data-ttu-id="fd821-200">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="fd821-200">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="fd821-201">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="fd821-201">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="fd821-202">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fd821-202">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fd821-203">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fd821-203">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="fd821-204">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="fd821-204">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="fd821-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd821-205">Response</span></span>
<span data-ttu-id="fd821-206">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd821-206">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd821-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd821-207">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd821-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd821-208">Request</span></span>
<span data-ttu-id="fd821-209">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd821-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1071

{
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

### <a name="response"></a><span data-ttu-id="fd821-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd821-210">Response</span></span>
<span data-ttu-id="fd821-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd821-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




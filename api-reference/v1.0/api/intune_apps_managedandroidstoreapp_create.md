# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="02acb-101">Criar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="02acb-101">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="02acb-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="02acb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02acb-103">Cria um novo objeto [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="02acb-103">Create a new [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="02acb-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02acb-104">Prerequisites</span></span>
<span data-ttu-id="02acb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="02acb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="02acb-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02acb-107">Permission type</span></span>|<span data-ttu-id="02acb-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02acb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02acb-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02acb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="02acb-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02acb-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="02acb-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02acb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02acb-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02acb-112">Not supported.</span></span>|
|<span data-ttu-id="02acb-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02acb-113">Application</span></span>|<span data-ttu-id="02acb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02acb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02acb-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02acb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="02acb-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02acb-116">Request headers</span></span>
|<span data-ttu-id="02acb-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02acb-117">Header</span></span>|<span data-ttu-id="02acb-118">Valor</span><span class="sxs-lookup"><span data-stu-id="02acb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02acb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="02acb-119">Authorization</span></span>|<span data-ttu-id="02acb-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02acb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02acb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="02acb-121">Accept</span></span>|<span data-ttu-id="02acb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="02acb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02acb-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02acb-123">Request body</span></span>
<span data-ttu-id="02acb-124">No corpo da solicitação, forneça uma representação JSON do objeto managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="02acb-124">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="02acb-125">A tabela a seguir mostra as propriedades obrigatórias ao criar managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="02acb-125">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="02acb-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02acb-126">Property</span></span>|<span data-ttu-id="02acb-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="02acb-127">Type</span></span>|<span data-ttu-id="02acb-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="02acb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02acb-129">id</span><span class="sxs-lookup"><span data-stu-id="02acb-129">id</span></span>|<span data-ttu-id="02acb-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02acb-130">String</span></span>|<span data-ttu-id="02acb-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="02acb-131">Key of the entity.</span></span> <span data-ttu-id="02acb-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02acb-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="02acb-133">displayName</span><span class="sxs-lookup"><span data-stu-id="02acb-133">displayName</span></span>|<span data-ttu-id="02acb-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02acb-134">String</span></span>|<span data-ttu-id="02acb-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="02acb-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="02acb-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02acb-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="02acb-137">description</span><span class="sxs-lookup"><span data-stu-id="02acb-137">description</span></span>|<span data-ttu-id="02acb-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02acb-138">String</span></span>|<span data-ttu-id="02acb-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02acb-139">The description of the app.</span></span> <span data-ttu-id="02acb-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02acb-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="02acb-141">publisher</span><span class="sxs-lookup"><span data-stu-id="02acb-141">publisher</span></span>|<span data-ttu-id="02acb-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02acb-142">String</span></span>|<span data-ttu-id="02acb-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02acb-143">The publisher of the app.</span></span> <span data-ttu-id="02acb-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02acb-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="02acb-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="02acb-145">largeIcon</span></span>|[<span data-ttu-id="02acb-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="02acb-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="02acb-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="02acb-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="02acb-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02acb-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="02acb-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02acb-149">createdDateTime</span></span>|<span data-ttu-id="02acb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02acb-150">DateTimeOffset</span></span>|<span data-ttu-id="02acb-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02acb-151">The date and time the app was created.</span></span> <span data-ttu-id="02acb-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02acb-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="02acb-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02acb-153">lastModifiedDateTime</span></span>|<span data-ttu-id="02acb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02acb-154">DateTimeOffset</span></span>|<span data-ttu-id="02acb-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="02acb-155">The date and time the app was last modified.</span></span> <span data-ttu-id="02acb-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02acb-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="02acb-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="02acb-157">isFeatured</span></span>|<span data-ttu-id="02acb-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="02acb-158">Boolean</span></span>|<span data-ttu-id="02acb-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02acb-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="02acb-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="02acb-160">privacyInformationUrl</span></span>|<span data-ttu-id="02acb-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02acb-161">String</span></span>|<span data-ttu-id="02acb-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="02acb-162">The privacy statement Url.</span></span> <span data-ttu-id="02acb-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02acb-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="02acb-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="02acb-164">informationUrl</span></span>|<span data-ttu-id="02acb-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02acb-165">String</span></span>|<span data-ttu-id="02acb-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="02acb-166">The more information Url.</span></span> <span data-ttu-id="02acb-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02acb-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="02acb-168">owner</span><span class="sxs-lookup"><span data-stu-id="02acb-168">owner</span></span>|<span data-ttu-id="02acb-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02acb-169">String</span></span>|<span data-ttu-id="02acb-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="02acb-170">The owner of the app.</span></span> <span data-ttu-id="02acb-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02acb-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="02acb-172">developer</span><span class="sxs-lookup"><span data-stu-id="02acb-172">developer</span></span>|<span data-ttu-id="02acb-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02acb-173">String</span></span>|<span data-ttu-id="02acb-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02acb-174">The developer of the app.</span></span> <span data-ttu-id="02acb-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02acb-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="02acb-176">notes</span><span class="sxs-lookup"><span data-stu-id="02acb-176">notes</span></span>|<span data-ttu-id="02acb-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02acb-177">String</span></span>|<span data-ttu-id="02acb-178">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02acb-178">Notes for the app.</span></span> <span data-ttu-id="02acb-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02acb-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="02acb-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="02acb-180">publishingState</span></span>|[<span data-ttu-id="02acb-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="02acb-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="02acb-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02acb-182">The publishing state for the app.</span></span> <span data-ttu-id="02acb-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="02acb-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="02acb-184">Herdada do [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02acb-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="02acb-185">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="02acb-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="02acb-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="02acb-186">appAvailability</span></span>|[<span data-ttu-id="02acb-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="02acb-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="02acb-188">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02acb-188">The Application's availability.</span></span> <span data-ttu-id="02acb-189">Herdada do [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="02acb-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md).</span></span> <span data-ttu-id="02acb-190">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="02acb-190">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="02acb-191">version</span><span class="sxs-lookup"><span data-stu-id="02acb-191">version</span></span>|<span data-ttu-id="02acb-192">String</span><span class="sxs-lookup"><span data-stu-id="02acb-192">String</span></span>|<span data-ttu-id="02acb-193">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02acb-193">The Application's version.</span></span> <span data-ttu-id="02acb-194">Herdado de [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="02acb-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="02acb-195">packageId</span><span class="sxs-lookup"><span data-stu-id="02acb-195">packageId</span></span>|<span data-ttu-id="02acb-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02acb-196">String</span></span>|<span data-ttu-id="02acb-197">A ID de pacote do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02acb-197">The app's package ID.</span></span>|
|<span data-ttu-id="02acb-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="02acb-198">appStoreUrl</span></span>|<span data-ttu-id="02acb-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02acb-199">String</span></span>|<span data-ttu-id="02acb-200">A AppStoreUrl do Android.</span><span class="sxs-lookup"><span data-stu-id="02acb-200">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="02acb-201">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="02acb-201">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="02acb-202">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="02acb-202">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="02acb-203">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="02acb-203">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="02acb-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="02acb-204">Response</span></span>
<span data-ttu-id="02acb-205">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02acb-205">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02acb-206">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02acb-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="02acb-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02acb-207">Request</span></span>
<span data-ttu-id="02acb-208">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02acb-208">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1016

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```

### <a name="response"></a><span data-ttu-id="02acb-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="02acb-209">Response</span></span>
<span data-ttu-id="02acb-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02acb-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1188

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```




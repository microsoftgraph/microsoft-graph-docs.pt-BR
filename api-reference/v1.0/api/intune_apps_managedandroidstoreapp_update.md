# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="59fca-101">Atualizar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="59fca-101">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="59fca-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="59fca-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59fca-103">Atualiza as propriedades de um objeto [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fca-103">Update the properties of a [calendar](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="59fca-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59fca-104">Prerequisites</span></span>
<span data-ttu-id="59fca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="59fca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="59fca-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59fca-107">Permission type</span></span>|<span data-ttu-id="59fca-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="59fca-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59fca-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59fca-109">Delegated (work or school account)</span></span>|<span data-ttu-id="59fca-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59fca-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="59fca-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59fca-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59fca-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59fca-112">Not supported.</span></span>|
|<span data-ttu-id="59fca-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59fca-113">Application</span></span>|<span data-ttu-id="59fca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59fca-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59fca-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59fca-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="59fca-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59fca-116">Request headers</span></span>
|<span data-ttu-id="59fca-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59fca-117">Header</span></span>|<span data-ttu-id="59fca-118">Valor</span><span class="sxs-lookup"><span data-stu-id="59fca-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59fca-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="59fca-119">Authorization</span></span>|<span data-ttu-id="59fca-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59fca-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="59fca-121">Accept</span><span class="sxs-lookup"><span data-stu-id="59fca-121">Accept</span></span>|<span data-ttu-id="59fca-122">application/json</span><span class="sxs-lookup"><span data-stu-id="59fca-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59fca-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59fca-123">Request body</span></span>
<span data-ttu-id="59fca-124">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fca-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="59fca-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fca-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="59fca-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59fca-126">Property</span></span>|<span data-ttu-id="59fca-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="59fca-127">Type</span></span>|<span data-ttu-id="59fca-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="59fca-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59fca-129">id</span><span class="sxs-lookup"><span data-stu-id="59fca-129">id</span></span>|<span data-ttu-id="59fca-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59fca-130">String</span></span>|<span data-ttu-id="59fca-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="59fca-131">Key of the setting.</span></span> <span data-ttu-id="59fca-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59fca-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59fca-133">displayName</span><span class="sxs-lookup"><span data-stu-id="59fca-133">displayName</span></span>|<span data-ttu-id="59fca-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59fca-134">String</span></span>|<span data-ttu-id="59fca-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="59fca-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="59fca-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59fca-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59fca-137">description</span><span class="sxs-lookup"><span data-stu-id="59fca-137">description</span></span>|<span data-ttu-id="59fca-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59fca-138">String</span></span>|<span data-ttu-id="59fca-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59fca-139">The description of the app.</span></span> <span data-ttu-id="59fca-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59fca-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59fca-141">publisher</span><span class="sxs-lookup"><span data-stu-id="59fca-141">Publisher</span></span>|<span data-ttu-id="59fca-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59fca-142">String</span></span>|<span data-ttu-id="59fca-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59fca-143">The publisher of the app.</span></span> <span data-ttu-id="59fca-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59fca-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59fca-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="59fca-145">largeIcon</span></span>|[<span data-ttu-id="59fca-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="59fca-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="59fca-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="59fca-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="59fca-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59fca-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59fca-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59fca-149">createdDateTime</span></span>|<span data-ttu-id="59fca-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59fca-150">DateTimeOffset</span></span>|<span data-ttu-id="59fca-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59fca-151">The date and time the group was created.</span></span> <span data-ttu-id="59fca-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59fca-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59fca-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59fca-153">lastModifiedDateTime</span></span>|<span data-ttu-id="59fca-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59fca-154">DateTimeOffset</span></span>|<span data-ttu-id="59fca-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="59fca-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="59fca-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59fca-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59fca-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="59fca-157">isFeatured</span></span>|<span data-ttu-id="59fca-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="59fca-158">Boolean</span></span>|<span data-ttu-id="59fca-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59fca-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59fca-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="59fca-160">privacyInformationUrl</span></span>|<span data-ttu-id="59fca-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59fca-161">String</span></span>|<span data-ttu-id="59fca-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="59fca-162">The privacy statement Url.</span></span> <span data-ttu-id="59fca-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59fca-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59fca-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="59fca-164">informationUrl</span></span>|<span data-ttu-id="59fca-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59fca-165">String</span></span>|<span data-ttu-id="59fca-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="59fca-166">The more information Url.</span></span> <span data-ttu-id="59fca-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59fca-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59fca-168">owner</span><span class="sxs-lookup"><span data-stu-id="59fca-168">owner</span></span>|<span data-ttu-id="59fca-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59fca-169">String</span></span>|<span data-ttu-id="59fca-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="59fca-170">The owner of the app.</span></span> <span data-ttu-id="59fca-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59fca-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59fca-172">developer</span><span class="sxs-lookup"><span data-stu-id="59fca-172">"developer"</span></span>|<span data-ttu-id="59fca-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59fca-173">String</span></span>|<span data-ttu-id="59fca-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59fca-174">The developer of the app.</span></span> <span data-ttu-id="59fca-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59fca-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59fca-176">notes</span><span class="sxs-lookup"><span data-stu-id="59fca-176">Notes</span></span>|<span data-ttu-id="59fca-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59fca-177">String</span></span>|<span data-ttu-id="59fca-178">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59fca-178">Notes for the app.</span></span> <span data-ttu-id="59fca-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59fca-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="59fca-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="59fca-180">publishingState</span></span>|<span data-ttu-id="59fca-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59fca-181">String</span></span>|<span data-ttu-id="59fca-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59fca-182">The publishing state for the app.</span></span> <span data-ttu-id="59fca-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="59fca-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="59fca-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os possíveis valores são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="59fca-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="59fca-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="59fca-185">appAvailability</span></span>|<span data-ttu-id="59fca-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59fca-186">String</span></span>|<span data-ttu-id="59fca-187">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59fca-187">The Application's availability.</span></span> <span data-ttu-id="59fca-188">Herdado de [managedApp](../resources/intune_apps_managedapp.md). Os possíveis valores são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="59fca-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="59fca-189">version</span><span class="sxs-lookup"><span data-stu-id="59fca-189">version</span></span>|<span data-ttu-id="59fca-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59fca-190">String</span></span>|<span data-ttu-id="59fca-191">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59fca-191">The Application's version.</span></span> <span data-ttu-id="59fca-192">Herdado de [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="59fca-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="59fca-193">packageId</span><span class="sxs-lookup"><span data-stu-id="59fca-193">packageId</span></span>|<span data-ttu-id="59fca-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59fca-194">String</span></span>|<span data-ttu-id="59fca-195">A ID de pacote do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59fca-195">The app's package ID.</span></span>|
|<span data-ttu-id="59fca-196">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="59fca-196">appStoreUrl</span></span>|<span data-ttu-id="59fca-197">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59fca-197">String</span></span>|<span data-ttu-id="59fca-198">A AppStoreUrl do Android.</span><span class="sxs-lookup"><span data-stu-id="59fca-198">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="59fca-199">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="59fca-199">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="59fca-200">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="59fca-200">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="59fca-201">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="59fca-201">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="59fca-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="59fca-202">Response</span></span>
<span data-ttu-id="59fca-203">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59fca-203">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59fca-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59fca-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="59fca-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59fca-205">Request</span></span>
<span data-ttu-id="59fca-206">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59fca-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1019

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

### <a name="response"></a><span data-ttu-id="59fca-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="59fca-207">Response</span></span>
<span data-ttu-id="59fca-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59fca-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




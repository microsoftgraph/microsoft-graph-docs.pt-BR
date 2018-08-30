# <a name="update-managediosstoreapp"></a><span data-ttu-id="2abf6-101">Atualizar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="2abf6-101">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="2abf6-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2abf6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2abf6-103">Atualiza as propriedades de um objeto [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="2abf6-103">Update the properties of a [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2abf6-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2abf6-104">Prerequisites</span></span>
<span data-ttu-id="2abf6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2abf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2abf6-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2abf6-107">Permission type</span></span>|<span data-ttu-id="2abf6-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2abf6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2abf6-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2abf6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2abf6-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2abf6-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2abf6-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2abf6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2abf6-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2abf6-112">Not supported.</span></span>|
|<span data-ttu-id="2abf6-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2abf6-113">Application</span></span>|<span data-ttu-id="2abf6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2abf6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2abf6-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2abf6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="2abf6-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2abf6-116">Request headers</span></span>
|<span data-ttu-id="2abf6-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2abf6-117">Header</span></span>|<span data-ttu-id="2abf6-118">Valor</span><span class="sxs-lookup"><span data-stu-id="2abf6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2abf6-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="2abf6-119">Authorization</span></span>|<span data-ttu-id="2abf6-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="2abf6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2abf6-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2abf6-121">Accept</span></span>|<span data-ttu-id="2abf6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2abf6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2abf6-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2abf6-123">Request body</span></span>
<span data-ttu-id="2abf6-124">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="2abf6-124">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.</span></span>

<span data-ttu-id="2abf6-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="2abf6-125">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).</span></span>

|<span data-ttu-id="2abf6-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2abf6-126">Property</span></span>|<span data-ttu-id="2abf6-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2abf6-127">Type</span></span>|<span data-ttu-id="2abf6-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2abf6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2abf6-129">id</span><span class="sxs-lookup"><span data-stu-id="2abf6-129">id</span></span>|<span data-ttu-id="2abf6-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2abf6-130">String</span></span>|<span data-ttu-id="2abf6-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2abf6-131">Key of the entity.</span></span> <span data-ttu-id="2abf6-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2abf6-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2abf6-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2abf6-133">displayName</span></span>|<span data-ttu-id="2abf6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2abf6-134">String</span></span>|<span data-ttu-id="2abf6-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="2abf6-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2abf6-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2abf6-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2abf6-137">description</span><span class="sxs-lookup"><span data-stu-id="2abf6-137">description</span></span>|<span data-ttu-id="2abf6-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2abf6-138">String</span></span>|<span data-ttu-id="2abf6-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2abf6-139">The description of the app.</span></span> <span data-ttu-id="2abf6-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2abf6-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2abf6-141">publicador</span><span class="sxs-lookup"><span data-stu-id="2abf6-141">publisher</span></span>|<span data-ttu-id="2abf6-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2abf6-142">String</span></span>|<span data-ttu-id="2abf6-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2abf6-143">The publisher of the app.</span></span> <span data-ttu-id="2abf6-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2abf6-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2abf6-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2abf6-145">largeIcon</span></span>|[<span data-ttu-id="2abf6-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2abf6-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="2abf6-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="2abf6-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2abf6-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2abf6-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2abf6-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2abf6-149">createdDateTime</span></span>|<span data-ttu-id="2abf6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2abf6-150">DateTimeOffset</span></span>|<span data-ttu-id="2abf6-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2abf6-151">The date and time the app was created.</span></span> <span data-ttu-id="2abf6-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2abf6-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2abf6-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2abf6-153">lastModifiedDateTime</span></span>|<span data-ttu-id="2abf6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2abf6-154">DateTimeOffset</span></span>|<span data-ttu-id="2abf6-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2abf6-155">The date and time the app was last modified.</span></span> <span data-ttu-id="2abf6-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2abf6-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2abf6-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2abf6-157">isFeatured</span></span>|<span data-ttu-id="2abf6-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="2abf6-158">Boolean</span></span>|<span data-ttu-id="2abf6-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2abf6-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2abf6-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2abf6-160">privacyInformationUrl</span></span>|<span data-ttu-id="2abf6-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2abf6-161">String</span></span>|<span data-ttu-id="2abf6-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="2abf6-162">The privacy statement Url.</span></span> <span data-ttu-id="2abf6-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2abf6-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2abf6-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2abf6-164">informationUrl</span></span>|<span data-ttu-id="2abf6-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2abf6-165">String</span></span>|<span data-ttu-id="2abf6-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="2abf6-166">The more information Url.</span></span> <span data-ttu-id="2abf6-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2abf6-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2abf6-168">owner</span><span class="sxs-lookup"><span data-stu-id="2abf6-168">owner</span></span>|<span data-ttu-id="2abf6-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2abf6-169">String</span></span>|<span data-ttu-id="2abf6-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2abf6-170">The owner of the app.</span></span> <span data-ttu-id="2abf6-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2abf6-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2abf6-172">desenvolvedor</span><span class="sxs-lookup"><span data-stu-id="2abf6-172">developer</span></span>|<span data-ttu-id="2abf6-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2abf6-173">String</span></span>|<span data-ttu-id="2abf6-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2abf6-174">The developer of the app.</span></span> <span data-ttu-id="2abf6-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2abf6-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2abf6-176">Observações</span><span class="sxs-lookup"><span data-stu-id="2abf6-176">notes</span></span>|<span data-ttu-id="2abf6-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2abf6-177">String</span></span>|<span data-ttu-id="2abf6-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2abf6-178">Notes for the app.</span></span> <span data-ttu-id="2abf6-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2abf6-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2abf6-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="2abf6-180">publishingState</span></span>|[<span data-ttu-id="2abf6-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2abf6-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="2abf6-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2abf6-182">The publishing state for the app.</span></span> <span data-ttu-id="2abf6-183">O aplicativo não pode ser atribuído, a menos que seja publicado.</span><span class="sxs-lookup"><span data-stu-id="2abf6-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2abf6-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2abf6-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="2abf6-185">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2abf6-185">The possible values are:</span></span>|
|<span data-ttu-id="2abf6-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="2abf6-186">appAvailability</span></span>|[<span data-ttu-id="2abf6-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="2abf6-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="2abf6-188">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2abf6-188">The Application's availability.</span></span> <span data-ttu-id="2abf6-189">Herdado de [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="2abf6-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span> <span data-ttu-id="2abf6-190">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="2abf6-190">The possible values are:</span></span>|
|<span data-ttu-id="2abf6-191">versão</span><span class="sxs-lookup"><span data-stu-id="2abf6-191">version</span></span>|<span data-ttu-id="2abf6-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2abf6-192">String</span></span>|<span data-ttu-id="2abf6-193">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2abf6-193">The Application's version.</span></span> <span data-ttu-id="2abf6-194">Herdado de [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="2abf6-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="2abf6-195">bundleId</span><span class="sxs-lookup"><span data-stu-id="2abf6-195">bundleId</span></span>|<span data-ttu-id="2abf6-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2abf6-196">String</span></span>|<span data-ttu-id="2abf6-197">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="2abf6-197">The app's Bundle ID.</span></span>|
|<span data-ttu-id="2abf6-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="2abf6-198">appStoreUrl</span></span>|<span data-ttu-id="2abf6-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2abf6-199">String</span></span>|<span data-ttu-id="2abf6-200">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="2abf6-200">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="2abf6-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="2abf6-201">applicableDeviceType</span></span>|[<span data-ttu-id="2abf6-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="2abf6-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="2abf6-203">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="2abf6-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="2abf6-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2abf6-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2abf6-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2abf6-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="2abf6-206">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="2abf6-206">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="2abf6-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="2abf6-207">Response</span></span>
<span data-ttu-id="2abf6-208">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2abf6-208">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2abf6-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2abf6-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="2abf6-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2abf6-210">Request</span></span>
<span data-ttu-id="2abf6-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2abf6-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2abf6-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="2abf6-212">Response</span></span>
<span data-ttu-id="2abf6-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2abf6-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




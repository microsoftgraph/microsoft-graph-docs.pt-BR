# <a name="create-iosstoreapp"></a><span data-ttu-id="8c99b-101">Criar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="8c99b-101">Create iosStoreApp</span></span>

> <span data-ttu-id="8c99b-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8c99b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c99b-103">Cria um novo objeto [iosStoreApp](../resources/intune_apps_iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="8c99b-103">Create a new [plannerBucket](../resources/intune_apps_iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c99b-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c99b-104">Prerequisites</span></span>
<span data-ttu-id="8c99b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8c99b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8c99b-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c99b-107">Permission type</span></span>|<span data-ttu-id="8c99b-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8c99b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c99b-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c99b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8c99b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c99b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8c99b-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c99b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c99b-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c99b-112">Not supported.</span></span>|
|<span data-ttu-id="8c99b-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c99b-113">Application</span></span>|<span data-ttu-id="8c99b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c99b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c99b-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c99b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8c99b-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c99b-116">Request headers</span></span>
|<span data-ttu-id="8c99b-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c99b-117">Header</span></span>|<span data-ttu-id="8c99b-118">Valor</span><span class="sxs-lookup"><span data-stu-id="8c99b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c99b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c99b-119">Authorization</span></span>|<span data-ttu-id="8c99b-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c99b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8c99b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8c99b-121">Accept</span></span>|<span data-ttu-id="8c99b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8c99b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c99b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c99b-123">Request body</span></span>
<span data-ttu-id="8c99b-124">No corpo da solicitação, forneça uma representação JSON do objeto iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="8c99b-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="8c99b-125">A tabela a seguir mostra as propriedades obrigatórias ao criar iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="8c99b-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="8c99b-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c99b-126">Property</span></span>|<span data-ttu-id="8c99b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c99b-127">Type</span></span>|<span data-ttu-id="8c99b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c99b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c99b-129">id</span><span class="sxs-lookup"><span data-stu-id="8c99b-129">id</span></span>|<span data-ttu-id="8c99b-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c99b-130">String</span></span>|<span data-ttu-id="8c99b-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8c99b-131">Key of the setting.</span></span> <span data-ttu-id="8c99b-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c99b-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8c99b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8c99b-133">displayName</span></span>|<span data-ttu-id="8c99b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c99b-134">String</span></span>|<span data-ttu-id="8c99b-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8c99b-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8c99b-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c99b-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8c99b-137">description</span><span class="sxs-lookup"><span data-stu-id="8c99b-137">description</span></span>|<span data-ttu-id="8c99b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c99b-138">String</span></span>|<span data-ttu-id="8c99b-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c99b-139">The description of the app.</span></span> <span data-ttu-id="8c99b-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c99b-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8c99b-141">publisher</span><span class="sxs-lookup"><span data-stu-id="8c99b-141">Publisher</span></span>|<span data-ttu-id="8c99b-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c99b-142">String</span></span>|<span data-ttu-id="8c99b-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c99b-143">The publisher of the app.</span></span> <span data-ttu-id="8c99b-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c99b-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8c99b-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8c99b-145">largeIcon</span></span>|[<span data-ttu-id="8c99b-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8c99b-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="8c99b-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="8c99b-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8c99b-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c99b-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8c99b-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c99b-149">createdDateTime</span></span>|<span data-ttu-id="8c99b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c99b-150">DateTimeOffset</span></span>|<span data-ttu-id="8c99b-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c99b-151">The date and time the group was created.</span></span> <span data-ttu-id="8c99b-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c99b-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8c99b-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c99b-153">lastModifiedDateTime</span></span>|<span data-ttu-id="8c99b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c99b-154">DateTimeOffset</span></span>|<span data-ttu-id="8c99b-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8c99b-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="8c99b-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c99b-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8c99b-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8c99b-157">isFeatured</span></span>|<span data-ttu-id="8c99b-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="8c99b-158">Boolean</span></span>|<span data-ttu-id="8c99b-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c99b-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8c99b-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8c99b-160">privacyInformationUrl</span></span>|<span data-ttu-id="8c99b-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c99b-161">String</span></span>|<span data-ttu-id="8c99b-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="8c99b-162">The privacy statement Url.</span></span> <span data-ttu-id="8c99b-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c99b-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8c99b-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8c99b-164">informationUrl</span></span>|<span data-ttu-id="8c99b-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c99b-165">String</span></span>|<span data-ttu-id="8c99b-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8c99b-166">The more information Url.</span></span> <span data-ttu-id="8c99b-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c99b-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8c99b-168">owner</span><span class="sxs-lookup"><span data-stu-id="8c99b-168">owner</span></span>|<span data-ttu-id="8c99b-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c99b-169">String</span></span>|<span data-ttu-id="8c99b-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8c99b-170">The owner of the app.</span></span> <span data-ttu-id="8c99b-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c99b-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8c99b-172">developer</span><span class="sxs-lookup"><span data-stu-id="8c99b-172">"developer"</span></span>|<span data-ttu-id="8c99b-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c99b-173">String</span></span>|<span data-ttu-id="8c99b-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c99b-174">The developer of the app.</span></span> <span data-ttu-id="8c99b-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c99b-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8c99b-176">notes</span><span class="sxs-lookup"><span data-stu-id="8c99b-176">Notes</span></span>|<span data-ttu-id="8c99b-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c99b-177">String</span></span>|<span data-ttu-id="8c99b-178">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c99b-178">Notes for the app.</span></span> <span data-ttu-id="8c99b-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c99b-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8c99b-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="8c99b-180">publishingState</span></span>|<span data-ttu-id="8c99b-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c99b-181">String</span></span>|<span data-ttu-id="8c99b-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c99b-182">The publishing state for the app.</span></span> <span data-ttu-id="8c99b-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="8c99b-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8c99b-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os possíveis valores são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8c99b-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8c99b-185">bundleId</span><span class="sxs-lookup"><span data-stu-id="8c99b-185">bundleId</span></span>|<span data-ttu-id="8c99b-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c99b-186">String</span></span>|<span data-ttu-id="8c99b-187">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="8c99b-187">The Identity Name.</span></span>|
|<span data-ttu-id="8c99b-188">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="8c99b-188">appStoreUrl</span></span>|<span data-ttu-id="8c99b-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c99b-189">String</span></span>|<span data-ttu-id="8c99b-190">A URL da Apple App Store</span><span class="sxs-lookup"><span data-stu-id="8c99b-190">The Apple App Store URL</span></span>|
|<span data-ttu-id="8c99b-191">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="8c99b-191">applicableDeviceType</span></span>|[<span data-ttu-id="8c99b-192">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="8c99b-192">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="8c99b-193">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="8c99b-193">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="8c99b-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8c99b-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8c99b-195">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8c99b-195">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="8c99b-196">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="8c99b-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="8c99b-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c99b-197">Response</span></span>
<span data-ttu-id="8c99b-198">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosStoreApp](../resources/intune_apps_iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c99b-198">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_apps_iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c99b-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c99b-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c99b-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c99b-200">Request</span></span>
<span data-ttu-id="8c99b-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c99b-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1050

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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

### <a name="response"></a><span data-ttu-id="8c99b-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c99b-202">Response</span></span>
<span data-ttu-id="8c99b-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c99b-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1158

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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




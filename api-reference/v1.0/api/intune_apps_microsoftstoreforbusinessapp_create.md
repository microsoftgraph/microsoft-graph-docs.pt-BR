# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="bdcd0-101">Criar microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="bdcd0-101">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="bdcd0-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdcd0-103">Cria um novo objeto [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="bdcd0-103">Create a new [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bdcd0-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bdcd0-104">Prerequisites</span></span>
<span data-ttu-id="bdcd0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bdcd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bdcd0-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdcd0-107">Permission type</span></span>|<span data-ttu-id="bdcd0-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdcd0-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bdcd0-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdcd0-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bdcd0-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdcd0-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-112">Not supported.</span></span>|
|<span data-ttu-id="bdcd0-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdcd0-113">Application</span></span>|<span data-ttu-id="bdcd0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdcd0-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdcd0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bdcd0-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdcd0-116">Request headers</span></span>
|<span data-ttu-id="bdcd0-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bdcd0-117">Header</span></span>|<span data-ttu-id="bdcd0-118">Valor</span><span class="sxs-lookup"><span data-stu-id="bdcd0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdcd0-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdcd0-119">Authorization</span></span>|<span data-ttu-id="bdcd0-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="bdcd0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdcd0-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bdcd0-121">Accept</span></span>|<span data-ttu-id="bdcd0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bdcd0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdcd0-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdcd0-123">Request body</span></span>
<span data-ttu-id="bdcd0-124">No corpo da solicitação, forneça uma representação JSON do objeto microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-124">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="bdcd0-125">A tabela a seguir mostra as propriedades obrigatórias ao criar microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-125">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="bdcd0-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdcd0-126">Property</span></span>|<span data-ttu-id="bdcd0-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdcd0-127">Type</span></span>|<span data-ttu-id="bdcd0-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdcd0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdcd0-129">id</span><span class="sxs-lookup"><span data-stu-id="bdcd0-129">id</span></span>|<span data-ttu-id="bdcd0-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdcd0-130">String</span></span>|<span data-ttu-id="bdcd0-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-131">Key of the entity.</span></span> <span data-ttu-id="bdcd0-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bdcd0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bdcd0-133">displayName</span></span>|<span data-ttu-id="bdcd0-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdcd0-134">String</span></span>|<span data-ttu-id="bdcd0-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bdcd0-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bdcd0-137">description</span><span class="sxs-lookup"><span data-stu-id="bdcd0-137">description</span></span>|<span data-ttu-id="bdcd0-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdcd0-138">String</span></span>|<span data-ttu-id="bdcd0-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-139">The description of the app.</span></span> <span data-ttu-id="bdcd0-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bdcd0-141">publicador</span><span class="sxs-lookup"><span data-stu-id="bdcd0-141">publisher</span></span>|<span data-ttu-id="bdcd0-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdcd0-142">String</span></span>|<span data-ttu-id="bdcd0-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-143">The publisher of the app.</span></span> <span data-ttu-id="bdcd0-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bdcd0-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bdcd0-145">largeIcon</span></span>|[<span data-ttu-id="bdcd0-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bdcd0-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="bdcd0-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bdcd0-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bdcd0-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bdcd0-149">createdDateTime</span></span>|<span data-ttu-id="bdcd0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdcd0-150">DateTimeOffset</span></span>|<span data-ttu-id="bdcd0-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-151">The date and time the app was created.</span></span> <span data-ttu-id="bdcd0-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bdcd0-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bdcd0-153">lastModifiedDateTime</span></span>|<span data-ttu-id="bdcd0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdcd0-154">DateTimeOffset</span></span>|<span data-ttu-id="bdcd0-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-155">The date and time the app was last modified.</span></span> <span data-ttu-id="bdcd0-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bdcd0-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bdcd0-157">isFeatured</span></span>|<span data-ttu-id="bdcd0-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="bdcd0-158">Boolean</span></span>|<span data-ttu-id="bdcd0-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bdcd0-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bdcd0-160">privacyInformationUrl</span></span>|<span data-ttu-id="bdcd0-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdcd0-161">String</span></span>|<span data-ttu-id="bdcd0-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-162">The privacy statement Url.</span></span> <span data-ttu-id="bdcd0-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bdcd0-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bdcd0-164">informationUrl</span></span>|<span data-ttu-id="bdcd0-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdcd0-165">String</span></span>|<span data-ttu-id="bdcd0-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-166">The more information Url.</span></span> <span data-ttu-id="bdcd0-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bdcd0-168">owner</span><span class="sxs-lookup"><span data-stu-id="bdcd0-168">owner</span></span>|<span data-ttu-id="bdcd0-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdcd0-169">String</span></span>|<span data-ttu-id="bdcd0-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-170">The owner of the app.</span></span> <span data-ttu-id="bdcd0-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bdcd0-172">developer</span><span class="sxs-lookup"><span data-stu-id="bdcd0-172">developer</span></span>|<span data-ttu-id="bdcd0-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdcd0-173">String</span></span>|<span data-ttu-id="bdcd0-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-174">The developer of the app.</span></span> <span data-ttu-id="bdcd0-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bdcd0-176">Observações</span><span class="sxs-lookup"><span data-stu-id="bdcd0-176">notes</span></span>|<span data-ttu-id="bdcd0-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdcd0-177">String</span></span>|<span data-ttu-id="bdcd0-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-178">Notes for the app.</span></span> <span data-ttu-id="bdcd0-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bdcd0-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="bdcd0-180">publishingState</span></span>|[<span data-ttu-id="bdcd0-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bdcd0-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="bdcd0-p114">O estado de publicação do aplicativo. O aplicativo não pode ser atribuído a menos que esteja publicado. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bdcd0-186">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="bdcd0-186">usedLicenseCount</span></span>|<span data-ttu-id="bdcd0-187">Int32</span><span class="sxs-lookup"><span data-stu-id="bdcd0-187">Int32</span></span>|<span data-ttu-id="bdcd0-188">O número de aplicativos da Microsoft Store for Business em uso.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-188">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="bdcd0-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="bdcd0-189">totalLicenseCount</span></span>|<span data-ttu-id="bdcd0-190">Int32</span><span class="sxs-lookup"><span data-stu-id="bdcd0-190">Int32</span></span>|<span data-ttu-id="bdcd0-191">O número total de aplicativos da Microsoft Store for Business.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-191">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="bdcd0-192">productKey</span><span class="sxs-lookup"><span data-stu-id="bdcd0-192">productKey</span></span>|<span data-ttu-id="bdcd0-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdcd0-193">String</span></span>|<span data-ttu-id="bdcd0-194">A chave de produto do aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdcd0-194">The app product key</span></span>|
|<span data-ttu-id="bdcd0-195">licenseType</span><span class="sxs-lookup"><span data-stu-id="bdcd0-195">licenseType</span></span>|[<span data-ttu-id="bdcd0-196">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="bdcd0-196">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune_apps_microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="bdcd0-p115">O tipo de licença do aplicativo Os valores possíveis são: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-p115">The app license type Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="bdcd0-199">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="bdcd0-199">packageIdentityName</span></span>|<span data-ttu-id="bdcd0-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdcd0-200">String</span></span>|<span data-ttu-id="bdcd0-201">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdcd0-201">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="bdcd0-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdcd0-202">Response</span></span>
<span data-ttu-id="bdcd0-203">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-203">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdcd0-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdcd0-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="bdcd0-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdcd0-205">Request</span></span>
<span data-ttu-id="bdcd0-206">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 833

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="bdcd0-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdcd0-207">Response</span></span>
<span data-ttu-id="bdcd0-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 941

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```








